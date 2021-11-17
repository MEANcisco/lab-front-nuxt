<template>
<div> 
    <LayoutLayHeader />

    <div class="rs-contact pt-120 md-pt-80">
                <div class="container">
                    <div class="row">
                        <div class="col-lg-4 md-mb-60">
                           <div class="contact-box">
                                <div class="sec-title mb-45">
                                    <span class="sub-text new-text white-color">Reservas</span>
                                    <h2 class="title white-color">Reserva tu visita.</h2>
                                </div>
                                <div class="address-box mb-25">
                                   <div :class="[step > 1 ? 'address-icon-active' : 'address-icon']">
                                       <no-ssr>
                                       <font-awesome-icon :style="{ color: '#fff' }" :icon="['fa', 'phone']"/> 
                                       </no-ssr>
                                   </div>
                                   <div class="address-text">
                                       <span class="label">Fecha de Reserva:</span>
                                       <a v-if="form.fechareserva.length">{{form.fechareserva}}</a>
                                   </div>
                                </div>
                                <div class="address-box mb-25">
                                   <div :class="[step > 2 ?   'address-icon-active' : 'address-icon']">
<no-ssr>
                                       <font-awesome-icon :style="{ color: '#fff' }" :icon="['fa', 'home']"/> 
                                       </no-ssr>
                                   </div>
                                   <div class="address-text">
                                        <span class="label">Informacion Paciente</span>
                                        <a >{{form.rut}}</a>
                                   </div>
                                </div>
                                <div class="address-box">
                                    <div :class="[step > 3 ? 'address-icon-active' : 'address-icon']">
<no-ssr>
                                       <font-awesome-icon :style="{ color: '#fff' }" :icon="['fa', 'map-marker']"/> 
                                       </no-ssr>
                                    </div>
                                    <div class="address-text">
                                       <span class="label">Finalización de Reserva:</span>
                                       <div class="desc"></div>
                                    </div>
                                </div>
                            </div>
                        </div> 
                        <div class="col-lg-8 pl-70 md-pl-15">
                            <div class="contact-widget">
                               <div class="sec-title2 mb-40">
                                   <span class="sub-text contact mb-15">Registro</span>
                                   <h2 v-if="step === 1" class="title testi-title" >Selecciona el día y hora </h2>
                                   <h2 v-if="step === 2" class="title testi-title">Añade algo de información</h2>
                                   <h2 v-if="step === 3" class="title testi-title">Hemos terminado!</h2>

                               </div>
                                <div id="form-messages"></div>
                                <form id="contact-form" method="post" action="mailer.php">
                                   <client-only> <fieldset v-if="step === 1">
                                        
                                        <VueCtkDateTimePicker v-model="form.fechareserva" :locale="'es-do'" :first-day-of-week="1" :min-date="to" :inline="true" :no-button-now="true"
                                        :minute-interval="10" :behaviour="{
    time: {
      nearestIfDisabled: true
    }
  }" :no-weekends-days="true" :disabled-hours="disabledHours" />
                                        
                                    </fieldset></client-only>
                                    <fieldset v-if="step === 2">
                                        <div class="row">
                                            
                                            <div class="col-lg-6 mb-30 col-md-6 col-sm-6">
                                                <input id="name" v-model="form.nombre" class="from-control" type="text" name="name" placeholder="Nombre" required="">
                                            </div> 
                                            <div class="col-lg-6 mb-30 col-md-6 col-sm-6">
                                                <input id="email" v-model="form.apellido" class="from-control" type="text" name="surname" placeholder="Apellido" required="">
                                            </div>   
                                            <div class="col-lg-6 mb-30 col-md-6 col-sm-6">
                                                <input id="rut" v-model="form.rut" class="from-control" type="text" name="rut" placeholder="Rut" required="" @input="CheckRut">
                                            </div> 
                                            <div class="col-lg-6 mb-30 col-md-6 col-sm-6">
                                                <input id="name" v-model="form.direccion" class="from-control" type="text" name="direccion" placeholder="direccion" required="">
                                            </div> 
                                            <div class="col-lg-6 mb-30 col-md-6 col-sm-6">
                                                <input id="email" v-model="form.correo" class="from-control" type="text" name="email" placeholder="Correo" required="">
                                            </div>   
                                            <div class="col-lg-6 mb-30 col-md-6 col-sm-6">
                                                <input id="telefono" v-model="form.telefono" class="from-control" type="text" name="phone" placeholder="Telefono" required="">
                                            </div>    
                                        </div>
                                        
                                    </fieldset>
                                    <div class="btn-part"> 
                                        <div class="row">
                                            <div class="form-group mb-0">
                                                <button v-if="step > 1" class="readon learn-more submit" type="submit" value="Volver" @click.prevent="backStep()">Volver</button>
                                            </div>                                           
                                            <div class="form-group mb-0">
                                                <button v-if="step !== totalSteps" class="readon learn-more submit" type="submit" value="Siguiente" @click.prevent="advanceStep()">Siguiente</button>
                                            </div>
                                        </div>
                                        </div> 
                                </form> 
                            </div>
                        </div>
                    </div>
                </div>
            </div>
</div>
</template>

<script>
import VueCtkDateTimePicker from 'vue-ctk-date-time-picker';
import 'vue-ctk-date-time-picker/dist/vue-ctk-date-time-picker.css';
import moment from 'moment';
import { format } from 'rut.js'
export default {
    components: {
        VueCtkDateTimePicker
    },
data: () => ({
    step: 1,
    totalSteps: 3,
    activeHour: false,
    pacientes: {},
    patientExists: false,
    pacienteDisponible: false,
    form: {
        fechareserva: '',
        nombre: '',
        apellido: '',
        rut: '',
        numero: '',
        correo: '',
        direccion: ''
    },
    to: moment().toISOString(),
    disabledDates: [ "2021-11-17" ], 
    enabledDates: [ "2021-02-21", "2021-02-22", "2021-02-23" ],
    disabledHours: ['00','01','02','03','04','05','06','07','19','20','21','22','23']

    }
    ),
    fetch() {
    this.$axios.$get('https://api.reservas-lab.ml/pacientes')
    .then(
        data => {
            this.pacientes = data; 
            console.log(this.pacientes);
        }
    )
    .catch(
        err => {
            // eslint-disable-next-line no-console
            console.error(err)
         }
    )
    // eslint-disable-next-line no-console
  },
methods: {
    CheckRut(){
        // eslint-disable-next-line no-console
        this.form.rut = format(this.form.rut);
         if(this.form.rut.length > 10) {
            this.rlnght = true
            console.log('mas de 10')
            
            const filteredDT = this.pacientes.filter( d => d.rut === this.form.rut);
            if(filteredDT.length){
                this.patientExists = true;
            } else {
                this.patientExists = false;
            }
    }
    },
    advanceStep() {
      this.step++;
      if(this.form.fechareserva) { 
          // eslint-disable-next-line no-console
          console.log(this.form.fechareserva)
          this.activeHour = true
      }
      // eslint-disable-next-line no-console
    },
    backStep() {
      this.step = this.step - 1
    }
  }
}
</script>