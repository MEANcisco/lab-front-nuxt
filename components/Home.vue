<template>
<div>
        <LayoutLayHeader />  
        <div class="main-content">
            
            <!--Full width header Start-->
          
            <!--Full width header End-->
         
            <!-- AQUI SLIDER -->
            <client-only>
                <div class="rs-slider style1" style="margin-top: 0px">
          
            <carousel class="rs-carousel" :rewind="true" :loop="true" :items="1" :margin="0" :autoplay-timeout="15000" :autoplay="true" :dots="false" :autoplay-hover-pause="true" :nav="true" :center="false"  >
                     <div class="slider-content slide2">
                        <div class="container">
                            <div class="content-part text-center">
                                <div class="sl-sub-title wow bounceInLeft" data-wow-delay="300ms" data-wow-duration="2000ms" style="text-shadow: 3px 3px 3px #000000;">Aumentamos la</div>
                                <h1 class="sl-title mb-mb-10 wow fadeInRight" data-wow-delay="600ms" data-wow-duration="2000ms" style="text-shadow: 3px 3px 3px #000000;">Calidad de exámenes</h1>
                                <div class="sl-desc fadeInUp" data-wow-delay="900ms" data-wow-duration="2000ms" style="text-shadow: 3px 3px 3px #000000;">
                                    Usando técnología moderna y lo ultimo en herramientas.
                                </div>
                                <ul class="slider-btn wow fadeInRight" data-wow-delay="200ms" data-wow-duration="3000ms">
                                    <li><a class="readon learn-more slider-btn" href="domicilios">Solicitar Domicilio</a></li>
                                    <li>
                                        <div class="slider-video">
                                            <a class="popup-videos" href="https://www.youtube.com/watch?v=ikMhfYguJ8k">
                                            <font-awesome-icon style="color: white" :icon="['fas', 'play']"/>              
                                             </a>
                                        </div>
                                    </li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    <div class="slider-content slide1">
                      <div class="container">
                            <div v-if="$device.isDesktop">  
                                <div class="row">
                        <div class="col-lg-6 col-md-12 pr-140 md-mb-140 md-pr-15">
                            <div class="content-wrap">
                                <h1 class="sl-title mb-mb-10 wow fadeInRight" data-wow-delay="600ms" style="text-shadow: 3px 3px 3px #000000;" data-wow-duration="2000ms">Laboratorio Clínico Alemán</h1>
                                <div class="description">
                                    <p  style=" color: #fff; text-shadow: 3px 3px 3px 3px #000000;">
Tecnología en analisis de muestras en la región del Maule.                                </p>
                                </div>
                            </div>
                        </div>
                        <div class="col-lg-6 col-md-12 pl-70 md-pl-15">

<div class="rs-contact">
                                <div class="contact-wrap">
                                   <div class="content-part mb-25">
                                       <h2 class="title mb-15">Horario de atención</h2>
                                       <p class="desc">Conoce nuestros horarios</p>
                                   </div>
                                    <div id="form-messages"></div>
                                    <form id="contact-form" method="post" action="mailer.php">
                                        <fieldset>
                                            <div class="row">
                                                <div class="col-lg-12 mb-15">
<div class="row">
                                                        <div class="col-lg-6"><h6 >Lunes a Viernes: </h6> </div>
                                                        <div class="col-lg-6"><p > 7:00am-7:00pm</p> </div>
                                                         
                                                    
                                                         </div>                                                </div> 
                                                <div class="col-lg-12 mb-15">
<div class="row">
                                                        <div class="col-lg-6"><h6 >Sabado: </h6> </div>
                                                        <div class="col-lg-6"><p > 7:00am-12:30pm</p> </div>
                                                         
                                                    
                                                         </div>                                                </div> 
                                                <div class="col-lg-12 mb-15">
                                                    <div class="row">
                                                        <div class="col-lg-6"><h6 >Domingo: </h6> </div>
                                                        <div class="col-lg-6" style="text-align: center"><p > Cerrado</p> </div>
                                                         
                                                    
                                                    </div>
                                                   
                                                    
                                                </div> 
                                            </div>
                                            <div class="form-group mb-0">
                                                <input class="submit-btn" type="submit" value="Reserva tu Hora">
                                            </div>
                                        </fieldset>
                                    </form> 
                                </div>
                            </div>  
                        </div>
                        </div> 
                            </div>
    <div v-else-if="$device.isTablet">
      <div class="row">
                        <div class="col-lg-6 col-md-12 pr-140 md-mb-140 md-pr-15">
                            <div class="content-wrap">
                                <h1 class="sl-title mb-mb-10 wow fadeInRight" data-wow-delay="600ms" style="text-shadow: 3px 3px 3px #000000;" data-wow-duration="2000ms">Laboratorio Clínico Alemán</h1>
                                <div class="description">
                                    <p  style=" color: #fff; text-shadow: 3px 3px 3px #000000;">
Tecnología en analisis de muestras en la región del Maule.                                </p>
                                </div>
                            </div>
                        </div>
                        <div class="col-lg-6 col-md-12 pl-70 md-pl-15">

<div class="rs-contact">
                                <div class="contact-wrap">
                                   <div class="content-part mb-25">
                                       <h2 class="title mb-15">Horario de atención</h2>
                                       <p class="desc">Conoce nuestros horarios</p>
                                   </div>
                                    <div id="form-messages"></div>
                                    <form id="contact-form" method="post" action="mailer.php">
                                        <fieldset>
                                            <div class="row">
                                                <div class="col-lg-12 mb-15">
<div class="row">
                                                        <div class="col-lg-6"><h6 >Lunes a Viernes: </h6> </div>
                                                        <div class="col-lg-6"><p > 7:00am-7:00pm</p> </div>
                                                         
                                                    
                                                         </div>                                                </div> 
                                                <div class="col-lg-12 mb-15">
<div class="row">
                                                        <div class="col-lg-6"><h6 >Sabado: </h6> </div>
                                                        <div class="col-lg-6"><p > 7:00am-12:30pm</p> </div>
                                                         
                                                    
                                                         </div>                                                </div> 
                                                <div class="col-lg-12 mb-15">
                                                    <div class="row">
                                                        <div class="col-lg-6"><h6 >Domingo: </h6> </div>
                                                        <div class="col-lg-6" style="text-align: center"><p > Cerrado</p> </div>
                                                         
                                                    
                                                    </div>
                                                   
                                                    
                                                </div> 
                                            </div>
                                            <div class="form-group mb-0">
                                                <input class="submit-btn" type="submit" value="Reserva tu Hora">
                                            </div>
                                        </fieldset>
                                    </form> 
                                </div>
                            </div>  
                        </div>
                        </div>
    </div>
    <div v-else>
        <div class="row">
            <div class="col-lg-12 col-md-12 pl-70 md-pl-15">

<div class="rs-contact">
                                <div class="contact-wrap">
                                   <div class="content-part mb-25">
                                       <h2 class="title mb-15">Horario de atención</h2>
                                       <p class="desc">Conoce nuestros horarios</p>
                                   </div>
                                    <div id="form-messages"></div>
                                    <form id="contact-form" method="post" action="mailer.php">
                                        <fieldset>
                                            <div class="row">
                                                <div class="col-lg-12 mb-15">
<div class="row">
                                                        <div class="col-lg-6"><h6 >Lunes a Viernes: </h6> </div>
                                                        <div class="col-lg-6"><p > 7:00am-7:00pm</p> </div>
                                                         
                                                    
                                                         </div>                                                </div> 
                                                <div class="col-lg-12 mb-15">
<div class="row">
                                                        <div class="col-lg-6"><h6 >Sabado: </h6> </div>
                                                        <div class="col-lg-6"><p > 7:00am-12:30pm</p> </div>
                                                         
                                                    
                                                         </div>                                                </div> 
                                                <div class="col-lg-12 mb-15">
                                                    <div class="row">
                                                        <div class="col-lg-6"><h6 >Domingo: </h6> </div>
                                                        <div class="col-lg-6" style="text-align: center"><p > Cerrado</p> </div>
                                                         
                                                    
                                                    </div>
                                                   
                                                    
                                                </div> 
                                            </div>
                                            <div class="form-group mb-0">
                                                <input class="submit-btn" type="submit" value="Reserva tu Hora">
                                            </div>
                                        </fieldset>
                                    </form> 
                                </div>
                            </div>  
                        </div>
        </div>
   </div>
                            
                        
                    
                        </div>
                    </div>
                   
            </carousel>
           
                </div>
            </client-only>
             <!-- Slider Section End -->

            <!-- Services Section Start -->
            
            <div v-if="$device.isMobile" style="margin-top: -50%" class="rs-services main-home style1 pt-100 " >
                <div class="container">
                    <div class="row">
                        
                        <div class="col-lg-3 col-md-6 md-mb-30">
                            <client-only>
                            <nuxt-link to="/reservas">
                           <div class="services-item">
                               <div class="services-icon">
                                   <div class="image-part">
                                       <img src="~static/reserva.svg" alt=""> 
                                   </div>
                               </div>
                               <div class="services-content">
                                   <div class="services-text">
                                       <h3 class="services-title"><a >Reserva Hora</a></h3>
                                   </div>
                                   <div class="services-desc">
                                       <p>
                                          Para asistir a la toma de exámenes
                                       </p>
                                   </div>
                               </div>
                           </div> 
                            </nuxt-link>
                            </client-only>
                        </div>
                        
                        <div class="col-lg-3 col-md-6 md-mb-30">
                            <client-only>
                                <nuxt-link to="/domicilios">
                            <div class="services-item">
                               <div class="services-icon">
                                   <div class="image-part">
                                       <img src="~static/domicilios.svg" alt="">  
                                   </div>
                               </div>
                               <div class="services-content">
                                   <div class="services-text">
                                       <h3 class="services-title"><a>Domicilios</a></h3>
                                   </div>
                                   <div class="services-desc">
                                       <p>
                                          Solicita un exámen a domicilio
                                       </p>
                                   </div>
                               </div>
                           </div> 
                                </nuxt-link>
                            </client-only>


                        </div>
                        <div class="col-lg-3 col-md-6 sm-mb-30">
                                <client-only>
                                <nuxt-link to="/domicilios">
                           <div class="services-item">
                               <div class="services-icon">
                                   <div class="image-part">
                                       <img src="~static/resultados.svg" alt="">  
                                   </div>
                               </div>
                               <div class="services-content">
                                   <div class="services-text">
                                       <h3 class="services-title"><a>Resultados</a></h3>
                                   </div>
                                   <div class="services-desc">
                                       <p>
                                         Revisa resultados de tus exámenes
                                       </p>
                                   </div>
                               </div>
                           </div> 
                                </nuxt-link>
                                </client-only>

                        </div>
                        <div class="col-lg-3 col-md-6">
                                <client-only>
                                <nuxt-link to="/domicilios">
                           <div class="services-item" >
                               <div class="services-icon">
                                   <div class="image-part">
                                       <img src="~static/cotizador.svg" alt=""> 
                                   </div>
                               </div>
                               <div class="services-content">
                                   <div class="services-text">
                                       <h3 class="services-title"><a >Cotizador</a></h3>
                                   </div>
                                   <div class="services-desc">
                                       <p>
                                          Revisa el valor de exámenes Fonasa.
                                       </p>
                                   </div>
                               </div>
                           </div> 
                                </nuxt-link>
                                </client-only>
                        </div>
                    </div>
                </div>
            </div>
            <div v-else class="rs-services main-home style1 pt-100 " >
           <div class="container">
                    <div class="row">
                        
                        <div class="col-lg-3 col-md-6 md-mb-30">
                            <client-only>
                            <nuxt-link to="/reservas">
                           <div class="services-item">
                               <div class="services-icon">
                                   <div class="image-part">
                                       <img src="~static/reserva.svg" alt=""> 
                                   </div>
                               </div>
                               <div class="services-content">
                                   <div class="services-text">
                                       <h3 class="services-title"><a >Reserva Hora</a></h3>
                                   </div>
                                   <div class="services-desc">
                                       <p>
                                          Para asistir a la toma de exámenes
                                       </p>
                                   </div>
                               </div>
                           </div> 
                            </nuxt-link>
                            </client-only>
                        </div>
                        
                        <div class="col-lg-3 col-md-6 md-mb-30">
                            <client-only>
                                <nuxt-link to="/domicilios">
                            <div class="services-item">
                               <div class="services-icon">
                                   <div class="image-part">
                                       <img src="~static/domicilios.svg" alt="">  
                                   </div>
                               </div>
                               <div class="services-content">
                                   <div class="services-text">
                                       <h3 class="services-title"><a>Domicilios</a></h3>
                                   </div>
                                   <div class="services-desc">
                                       <p>
                                          Solicita un exámen a domicilio
                                       </p>
                                   </div>
                               </div>
                           </div> 
                                </nuxt-link>
                            </client-only>


                        </div>
                        <div class="col-lg-3 col-md-6 sm-mb-30">
                                <client-only>
                                <nuxt-link to="/resultados">
                           <div class="services-item">
                               <div class="services-icon">
                                   <div class="image-part">
                                       <img src="~static/resultados.svg" alt="">  
                                   </div>
                               </div>
                               <div class="services-content">
                                   <div class="services-text">
                                       <h3 class="services-title"><a>Resultados</a></h3>
                                   </div>
                                   <div class="services-desc">
                                       <p>
                                         Revisa resultados de tus exámenes
                                       </p>
                                   </div>
                               </div>
                           </div> 
                                </nuxt-link>
                                </client-only>

                        </div>
                        <div class="col-lg-3 col-md-6">
                                <client-only>
                                <nuxt-link to="/domicilios">
                           <div class="services-item" >
                               <div class="services-icon">
                                   <div class="image-part">
                                       <img src="~static/cotizador.svg" alt=""> 
                                   </div>
                               </div>
                               <div class="services-content">
                                   <div class="services-text">
                                       <h3 class="services-title"><a >Cotizador</a></h3>
                                   </div>
                                   <div class="services-desc">
                                       <p>
                                          Revisa el valor de exámenes Fonasa.
                                       </p>
                                   </div>
                               </div>
                           </div> 
                                </nuxt-link>
                                </client-only>
                        </div>
                    </div>
                </div>
            </div>
            <!-- Services Section End -->

            <!-- About Section Start -->
            <div id="nosotros" class="rs-about bg4 pt-120 pb-120 md-pt-80 md-pb-80">
                <div class="container">
                    <div class="row align-items-center">
                        <div class="col-lg-6 md-mb-50">
                            <div class="images">
                               <img src="~/assets/images/about/about-2.png" alt=""> 
                            </div> 
                        </div>
                        <div class="col-lg-6 pl-60 md-pl-15">
                            <div class="contact-wrap">
                                <div class="sec-title mb-30">
                                    <div class="sub-text style2">Sobre Nosotros</div>
                                    <h2 class="title pb-38">
                                        Laboratorio Clínico Alemán
                                    </h2>
                                    <div class="desc pb-35">
                                       Descripción de prueba lorem ipsum dolor sit amet.
                                    </div>
                                    <p class="margin-0 pb-15">
                                      Subtitulo lorem ipsum dolor sit amet.
                                    </p>
                                </div>
                                <div class="btn-part">
                                    <a class="readon learn-more contact-us" href="contact.html">Ver Más</a>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <!-- About Section End -->

            
            <!-- Call Us Section Start -->

            <!-- Counter Section Start -->
            <div class="rs-counter main-counter-home">
                 <div class="counter-top-area text-center bg2">
                     <div class="row">
                         <div class="col-lg-4 md-mb-40">
                             <div class="counter-list">
                                 <div class="counter-text">
                                     <div class="count-number">
                                         <span class="rs-count k">80</span>
                                     </div>
                                     <h3 class="title">Clientes</h3>
                                 </div>
                             </div>
                         </div>
                         <div class="col-lg-4 md-mb-40">
                             <div class="counter-list">
                                 <div class="counter-text">
                                     <div class="count-number">
                                         <span class="rs-count plus">50</span>
                                     </div>
                                     <h3 class="title">Examenes</h3>
                                 </div>
                             </div>
                         </div>
                         <div class="col-lg-4">
                             <div class="counter-list">
                                 <div class="counter-text">
                                     <div class="count-number">
                                         <span class="rs-count plus">230</span>
                                     </div>
                                     <h3 class="title">Experiencia</h3>
                                 </div>
                             </div>
                         </div>
                     </div> 
                 </div>
            </div>
            <!-- Counter Section End -->

            <!-- Process Section Start -->
            <div class="rs-process pt-180 pb-120 md-pt-80 md-pb-80">
                <div class="container">
                    <div class="row align-items-center">
                        <div class="col-lg-4 md-mb-40">
                            <div class="process-wrap bg3">
                                <div class="sec-title mb-30">
                                    <div class="sub-text new">Toma de exámenes</div>
                                    <h2 class="title white-color">
                                        Indicaciones Exámenes de Laboratorio
                                    </h2>
                                </div>
                                <div class="btn-part mt-40">
                                    <a class="readon learn-more contact-us" href="#footer">Contactar</a>
                                </div>
                            </div>
                        </div>
                        <div class="col-lg-8 pl-30 md-pl-15">
                            <div class="row">
                                <div class="col-lg-6 col-md-6 mb-40">
                                    <div class="rs-addon-number">
                                        <div class="number-text">
                                            <div class="number-area">
                                                1.
                                            </div>
                                            <div class="number-title">
                                                <h3 class="title"> Investiga</h3>
                                            </div>
                                            <p class="number-txt">  Mantente informado de el tipo de examen a realizar, si se toma de ayunas, en la mañana o diversas indicaciones, a veces no existen indicaciones.</p>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-lg-6 col-md-6 mb-40">
                                    <div class="rs-addon-number">
                                        <div class="number-text">
                                            <div class="number-area">
                                                2.
                                            </div>
                                            <div class="number-title">
                                                <h3 class="title">Visita</h3>
                                            </div>
                                            <p class="number-txt">Puedes ir directamente a la sucursal o reservar tu hora por internet, es importante ser consciente de la hora para evitar aglomeraciones y no tomar medidas innecesarias.</p>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-lg-6 col-md-6 sm-mb-40">
                                    <div class="rs-addon-number">
                                        <div class="number-text">
                                            <div class="number-area">
                                                3.
                                            </div>
                                            <div class="number-title">
                                                <h3 class="title">Muestra</h3>
                                            </div>
                                            <p class="number-txt">Una vez la visita se haya realizado, un profesional de la salud tomará la muestra necesaria para el exámen.</p>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-lg-6 col-md-6">
                                    <div class="rs-addon-number">
                                        <div class="number-text">
                                            <div class="number-area">
                                                4.
                                            </div>
                                            <div class="number-title">
                                                <h3 class="title">Resultado</h3>
                                            </div>
                                            <p class="number-txt">Puedes revisar tu resultado en linea click en "Resultados", también se puede hacer de forma presencial.</p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <!-- Process Section End -->

            <!-- Blog Section Start -->
            <div id="rs-blog" class="rs-blog pb-120 pt-120 md-pt-80 md-pb-80">
                <div class="container">  
                    <div class="sec-title2 text-center mb-45">
                        <span class="sub-text">Blogs</span>
                            <h2 class="title testi-title">
                                Vea nuestro blog informativo
                            </h2>
                        <div class="heading-line">

                        </div>
                    </div>
                       <client-only>
          
            <carousel class="rs-carousel" :rewind="true" :loop="true" :items="3" :margin="30" :autoplay="true" :dots="false" :nav="true" :center="false"  >
                        <div class="blog-item">
                            <div class="image-wrap">
                                <a href="blog-details.html"><img src="~/assets/images/blog/main-home/1.jpg" alt=""></a>
                                <ul class="post-categories">
                                    <li><a href="blog-details.html">Técnología</a></li>
                                </ul>
                            </div>
                            <div class="blog-content">
                               <ul class="blog-meta">
                                   <li class="date"><i class="fa fa-calendar-check-o"></i> 16 Nov 2020</li>
                                   <li class="admin"><i class="fa fa-user-o"></i> admin</li>
                               </ul>
                               <h3 class="blog-title"><a href="blog-details.html">Toma de muestras efectiva</a></h3>
                               <p class="desc">¿Como tomar una buena muestra?...</p>
                               <div class="blog-button"><a href="blog-details.html">Ver más</a></div>
                            </div>
                        </div>

                        <div class="blog-item">
                            <div class="image-wrap">
                                <a href="blog-details.html"><img src="~/assets/images/blog/main-home/1.jpg" alt=""></a>
                                <ul class="post-categories">
                                    <li><a href="blog-details.html">Salud</a></li>
                                </ul>
                            </div>
                            <div class="blog-content">
                               <ul class="blog-meta">
                                   <li class="date"><i class="fa fa-calendar-check-o"></i> 16 Nov 2020</li>
                                   <li class="admin"><i class="fa fa-user-o"></i> admin</li>
                               </ul>
                               <h3 class="blog-title"><a href="blog-details.html">Coronavirus</a></h3>
                               <p class="desc">¿Que tipo de exámen debo tomar?...</p>
                               <div class="blog-button"><a href="blog-details.html">Ver más</a></div>
                            </div>
                        </div>
                       
            </carousel>
                       </client-only>
                </div>
            </div>
            <!-- Blog Section End -->

            <!-- Partner Start -->
            <div class="rs-partner pt-80 pb-70">
                <div class="container">
                       <client-only>          
            <carousel class="rs-carousel" :rewind="true" :loop="true" :items="5" :margin="30" :autoplay="true" :dots="false" :nav="true" :center="false"  >
                        <div class="partner-item">
                            <div class="logo-img">
                                <a href="https://rstheme.com">
                                    <img class="hover-logo" src="~/assets/images/partner/1.png" alt="">
                                    <img class="main-logo" src="~/assets/images/partner/1.png" alt="">
                                </a>
                            </div>
                        </div>
                        <div class="partner-item">
                            <div class="logo-img">
                                <a href="https://rstheme.com">
                                    <img class="hover-logo" src="~/assets/images/partner/2.png" alt="">
                                    <img class="main-logo" src="~/assets/images/partner/2.png" alt="">
                                </a>
                            </div>
                        </div>
                        <div class="partner-item">
                            <div class="logo-img">
                                <a href="https://rstheme.com">
                                    <img class="hover-logo" src="~/assets/images/partner/3.png" alt="">
                                    <img class="main-logo" src="~/assets/images/partner/3.png" alt="">
                                </a>
                            </div>
                        </div>
                        <div class="partner-item">
                            <div class="logo-img">
                                <a href="https://rstheme.com">
                                    <img class="hover-logo" src="~/assets/images/partner/4.png" alt="">
                                    <img class="main-logo" src="~/assets/images/partner/4.png" alt="">
                                </a>
                            </div>
                        </div>
                        <div class="partner-item">
                            <div class="logo-img">
                                <a href="https://rstheme.com">
                                    <img class="hover-logo" src="~/assets/images/partner/5.png" alt="">
                                    <img class="main-logo" src="~/assets/images/partner/5.png" alt="">
                                </a>
                            </div>
                        </div>
                        <div class="partner-item">
                            <div class="logo-img">
                                <a href="https://rstheme.com">
                                    <img class="hover-logo" src="~/assets/images/partner/6.png" alt="">
                                    <img class="main-logo" src="~/assets/images/partner/6.png" alt="">
                                </a>
                            </div>
                        </div>
                        <div class="partner-item">
                            <div class="logo-img">
                                <a href="https://rstheme.com">
                                    <img class="hover-logo" src="~/assets/images/partner/7.png" alt="">
                                    <img class="main-logo" src="~/assets/images/partner/7.png" alt="">
                                </a>
                            </div>
                        </div>
                        <div class="partner-item">
                            <div class="logo-img">
                                <a href="https://rstheme.com">
                                    <img class="hover-logo" src="~/assets/images/partner/8.png" alt="">
                                    <img class="main-logo" src="~/assets/images/partner/8.png" alt="">
                                </a>
                            </div>
                        </div>
                        <div class="partner-item">
                            <div class="logo-img">
                                <a href="https://rstheme.com">
                                    <img class="hover-logo" src="~/assets/images/partner/9.png" alt="">
                                    <img class="main-logo" src="~/assets/images/partner/9.png" alt="">
                                </a>
                            </div>
                        </div>
            </carousel>
                       </client-only>
                </div>
            </div>
            <!-- Partner End -->

        </div> 
        <LayoutLayFooter />
</div>
</template>

<script>
export default {
    setup() {
        
    },
    methods: {}
}
</script>
