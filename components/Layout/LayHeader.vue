<template>
<div class="full-width-header">

        <header id="rs-header" class="rs-header">
                    <!-- Topbar Area Start -->
                    <div class="topbar-area" >
                        <div class="container">
                            <div class="row rs-vertical-middle">
                                <div class="col-lg-2">
                                    <div class="logo-part">
                                        <a href="index.html"><img src="~static/logo.svg" alt=""></a>
                                    </div>
                                </div>
                                <div class="col-lg-10 text-right" style="border-bottom: 1px solid #3E5274;">
                                    <ul class="rs-contact-info">
                                        <li class="contact-part">
                                            <i class="flaticon-location"></i>
                                            <span class="contact-info">
                                                <span>Dirección</span>
                                                Manuel Montt 387, Curicó, Maule
                                            </span>
                                        </li>
                                        <li class="contact-part">
                                            <i class="flaticon-email"></i>
                                            <span class="contact-info">
                                                <span>E-mail</span>
                                                <a> contacto@laboratorioaleman.cl</a>
                                            </span>
                                        </li>
                                        <li class="contact-part no-border">
                                             <i class="flaticon-call"></i>
                                            <span class="contact-info">
                                                <span>Telefono</span>
                                                 +56 75 232 3749
                                            </span>
                                        </li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>
                    <!-- Topbar Area End -->

                    <!-- Menu Start -->
                    <div class="menu-area menu-sticky">
                        <div class="container">
                            <div class="logo-area">
                                <a href="/">
                                    <img class="sticky-logo" src="~static/logo.svg" alt="logo">
                                </a>
                            </div>
                            <div class="rs-menu-area">
                                <div class="main-menu">
                                    <div class="mobile-menu" style="border-bottom: 1px solid #3E5274;">
                                        <a href="/" class="mobile-logo">
                                            <img style="height: 80px" src="~static/logo.svg" alt="logo">
                                        </a>
                                        <a class="rs-menu-toggle rs-menu-toggle-close"  @click="toggleClass()">
<font-awesome-icon :style="{ color: 'black' }" :icon="['fa', 'bars']"/>                                        </a>
                                    </div>

                                    <nav v-if="$device.isDesktop" style="margin-left: 55%" :class="[isActive ? 'rs-menu-open' : 'rs-menu-close']" class="rs-menu ">
                                        <ul id="onepage-menu" class="nav-menu">
                                            <li style="margin-right: 0px"> 
                                                <client-only>
                                                    <nuxt-link to="/">
                                                <a style="font-family:'DIN Alternate Bold';font-weight:normal; font-size:18px; color: #53575A">INICIO</a>
                                                    </nuxt-link>
                                                </client-only>
                                            </li>

                                            <li style="margin-right: 0px"> 
                                                <client-only>
                                                    <nuxt-link to="/reservas">
                                                <a style="font-family:'DIN Alternate Bold';font-weight:normal; font-size:18px; color: #53575A">RESERVA HORAS</a>
                                                    </nuxt-link>
                                                </client-only>
                                            </li>

                                            <li style="margin-right: 0px"> 
                                                <client-only>
                                                    <nuxt-link to="/domicilios">
                                                <a style="font-family:'DIN Alternate Bold';font-weight:normal; font-size:18px; color: #53575A">DOMICILIO</a>
                                                    </nuxt-link>
                                                </client-only>
                                            </li>

                                            <li style="margin-right: 0px"> 
                                                <client-only>
                                                    <nuxt-link to="/resultados">
                                                    <a style="font-family:'DIN Alternate Bold';font-weight:normal; font-size:18px; color: #53575A">RESULTADOS</a>
                                                    </nuxt-link>
                                                </client-only>
                                            </li>
                                            <li style="margin-right: 0px"> 
                                                <client-only>
                                                    <nuxt-link to="/cotizador">
                                                <a style="font-family:'DIN Alternate Bold';font-weight:normal; font-size:18px; color: #53575A">COTIZADOR</a>
                                                    </nuxt-link>
                                                </client-only>
                                            </li>
                                            <li style="margin-right: 0px"> 
                                                <client-only>
                                                    <nuxt-link to="#nosotros">
                                                <a  style="font-family:'DIN Alternate Bold';font-weight:normal; font-size:18px; color: #53575A">NOSOTROS</a>
                                                    </nuxt-link>
                                                </client-only>
                                            </li>
                                            <li>
                                                <client-only>
                                                <nuxt-link to="#footer">
                                                <a style="font-family:'DIN Alternate Bold';font-weight:normal; font-size:18px; color: #53575A">CONTACTO</a>
                                                </nuxt-link>
                                                </client-only>
                                            </li>
                                        </ul> <!-- //.nav-menu -->
                                    </nav>
                                    <nav v-if="$device.isMobile"  :class="[isActive ? 'rs-menu-open' : 'rs-menu-close']" class="rs-menu ">
                                        <ul id="onepage-menu" class="nav-menu">
                                            <li> 
                                                <client-only>
                                                    <nuxt-link to="/">
                                                <a style="font-family:'DIN Alternate Bold';font-weight:normal; font-size:18px; color: #53575A">INICIO</a>
                                                    </nuxt-link>
                                                </client-only>
                                            </li>

                                            <li>
                                                <client-only>
                                                    <nuxt-link to="/reservas">
                                                <a style="font-family:'DIN Alternate Bold';font-weight:normal; font-size:18px; color: #53575A">RESERVA HORAS</a>
                                                    </nuxt-link>
                                                </client-only>
                                            </li>

                                            <li> 
                                                <client-only>
                                                    <nuxt-link to="/domicilios">
                                                <a style="font-family:'DIN Alternate Bold';font-weight:normal; font-size:18px; color: #53575A">DOMICILIO</a>
                                                    </nuxt-link>
                                                </client-only>
                                            </li>

                                            <li>
                                                <client-only>
                                                    <nuxt-link to="/resultados">
                                                <a style="font-family:'DIN Alternate Bold';font-weight:normal; font-size:18px; color: #53575A">RESULTADOS</a>
                                                    </nuxt-link>
                                                </client-only>
                                            </li>
                                            <li>
                                                <client-only>
                                                    <nuxt-link to="/cotizador">
                                                <a style="font-family:'DIN Alternate Bold';font-weight:normal; font-size:18px; color: #53575A">COTIZADOR</a>
                                                    </nuxt-link>
                                                </client-only>
                                            </li>
                                            <li>
                                                <client-only>
                                                    <nuxt-link to="/nosotros">
                                                <a style="font-family:'DIN Alternate Bold';font-weight:normal; font-size:18px; color: #53575A">NOSOTROS</a>
                                                    </nuxt-link>
                                                </client-only>
                                            </li>
                                            <li>
                                                <a href="#footer" style="font-family:'DIN Alternate Bold';font-weight:normal; font-size:18px; color: #53575A">CONTACTO</a>
                                            </li>
                                        </ul> <!-- //.nav-menu -->
                                    </nav>                                
                                </div> <!-- //.main-menu -->                                
                            </div>
                            <div class="expand-btn-inner search-icon hidden-sticky hidden-md">
                                <ul>
                                    
                                </ul>
                                
                            </div>
                        </div>
                    </div>
                    <!-- Menu End -->
                </header>
</div>
</template>


<script>
export default {
     data() {
return {
    isActive: false
  };
},
  methods: {
    toggleClass(){
       this.isActive = !this.isActive;
    }
  }
}
</script>