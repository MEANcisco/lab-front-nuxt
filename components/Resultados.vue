<template>
        <div>       
            <LayoutLayHeader /> 
            <no-ssr>                                          
            <div class="rs-banner style3 rs-rain-animate modify1">
                <div class="container">
                    <div class="row">
                        <div class="col-lg-6">
                            <div class="banner-content">
                                <div class="rs-videos">
                                    <div class="animate-border white-color style3">
                                        <nuxt-link to="/">
                                        <a class="popup-border popup-videos" >
                                            <font-awesome-icon style="color: #a21a5b" :icon="['fas', 'arrow-left']"/>              
                                        </a>
                                        </nuxt-link>
                                    </div>
                                </div> 
                               <h1 class="title">Revisa tus exámenes en linea </h1>
                                <p class="desc">
                                   Ingresa la información entregada a la hora de atenderte en el formulario, podrás ver el estado de tus exámenes.
                                </p>
                              
                            </div>
                        </div>
                        <div class="col-lg-6">
                            <client-only>
                            <form class="form-horizontal content-form" name="MainGST" method="POST" action="http://45.71.46.202/irispacientes/login_nuevo2.asp">
                            <div class="col-md-10 col-md-offset-1">
                                                    <h3 style="color: #ffffff">Información de atención</h3>
                                                </div>
 <div class="form-group">
                                                <div class="col-md-10 col-md-offset-1">
<input class="form-control" name="fsRut" type="text" onchange="checkRutField(fsRut.value)" size="15" maxlength="15" csize="10" placeholder="RUT"> 
</div></div>
<div class="form-group">
                                                <div class="col-md-10 col-md-offset-1"><input id="I_Num" class="form-control" name="I_Num" type="text"  size="10" maxlength="15" placeholder="N° de folio"> 
</div></div>
                <div class="form-group">
                                                <div class="col-md-10 col-md-offset-1">
                                                    <label style="color: #ffffff">Fecha de toma de muestras</label>
                                                </div>
                                                <div class="col-md-10 col-md-offset-1"> 
				 <input id="inputFechaToma" name="inputFechaToma"  type="date" class="form-control"> 
					  </div>
                                            </div>				

					  <div class="form-group">
                                                <div class="col-md-10 col-md-offset-1">
                                                    <button type="submit" class="btn btn-danger" style="4dth:100%;">Entrar</button>
                                                </div>  
                                            </div>
           

  <p style=" text-align:center;"><font face="Arial, Helvetica" color="#ffffff" size="1"> 
	<script language="JavaScript" src="Java/dia.js" scr="js/dia.js">
	</script>Miércoles 10 de Noviembre, 2021
	 <br>
    © 2010 - www.IrisLAB.cl </font></p>
 </form>
 </client-only>
                        </div>
                    </div>
                </div>                
                <div class="images-part hidden-md">
                    <img src="assets/images/banner/banner-4.png" alt="">
                </div>
                <div class="line-inner style2">
                    <div class="line"></div>
                    <div class="line"></div>
                    <div class="line"></div>
                </div>
            </div>
            </no-ssr>
        </div> 
</template> 
