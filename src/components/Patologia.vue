<template lang="html">
  <div>
    <v-container>
      <h2 class="title_slider">title <a class="title_slider_more">mas</a></h2>
    </v-container>
    <v-layout row>
      <v-carousel class="carousel_master_p">
        <v-carousel-item>
          <v-container>
            <v-layout>
              <v-flex xs12 sm3 sm3 class="p10">
                <v-card>
                  <img class="resposive_img" src="@/assets/pato.png" width="100%">
                  <a href="#">
                    <div class="pat_box">
                      Vitaminas <i class="icon material-icons">chevron_right</i>
                    </div>
                  </a>
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>
         </v-carousel-item>
       </v-carousel>
     </v-layout>
     <br>

    <section class="section-b">
     <v-container>
       <h2 class="title_slider">title <a class="title_slider_more">mas</a></h2>
     </v-container>
     <v-layout row>
       <v-carousel class="carousel_master_p">
         <v-carousel-item>
           <v-container>
             <v-layout>
               <v-flex xs12 sm3 sm3 class="p10">
                 <v-card class="box_marca">
                   <img class="resposive_img" src="@/assets/marca.png" width="100%">
                 </v-card>
               </v-flex>
             </v-layout>
           </v-container>
          </v-carousel-item>
        </v-carousel>
      </v-layout>
    </section>

    <section>
     <v-container>
       <h2 class="title_slider">title <a class="title_slider_more">mas</a></h2>
     </v-container>
     <v-layout row>
       <v-carousel class="carousel_master_p">
         <v-carousel-item>
           <v-container>
             <v-layout>
               <v-flex xs12 sm6 sm6 class="p10">
                 <v-layout row wrap>
                  <v-flex xs12 sm2 sm2 class="p10 center">
                    <img class="resposive_img img_testimoneo" src="@/assets/testimo.png" width="100%">
                  </v-flex>
                  <v-flex xs12 sm10 sm10>
                    <h3 class="title_testimoneo">title</h3>
                    <p class="title_testimoneo_2">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
                  </v-flex>
                 </v-layout>
               </v-flex>
               <v-flex xs12 sm6 sm6 class="p10">
                 <v-layout row wrap>
                  <v-flex xs12 sm2 sm2 class="p10 center">
                    <img class="resposive_img img_testimoneo" src="@/assets/testimo.png" width="100%">
                  </v-flex>
                  <v-flex xs12 sm10 sm10>
                    <h3 class="title_testimoneo">title</h3>
                    <p class="title_testimoneo_2">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
                  </v-flex>
                 </v-layout>
               </v-flex>
             </v-layout>
           </v-container>
          </v-carousel-item>
        </v-carousel>
      </v-layout>
    </section>

  </div>
</template>

<script>
export default {
  data () {
    return {
      // /* DETALLE DEL PRODUCTO */
      active: null,
      text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.',
      /* STEPEER */
      e1: 0

    }
  }
}
</script>

<style>
.carousel_master_p{
  height: auto;
  box-shadow: none;
}
.carousel_master_p .carousel__right {
    right: 5px;
    border-radius: 50%;
    background: #ddd;
}
.carousel_master_p .carousel__left {
    left: 5px;
    border-radius: 50%;
    background: #ddd;
}
.carousel_master_p .carousel__controls{
  display: none!important;
}
.title_slider{
  color: #268ae0;
  font-weight: 700;
}
.title_slider_more{
  color: #fd5621;
  font-size: 13px;
  font-weight: 200;
}
.pat_box{
  background: #f4f4f4;
  color: #268ae0;
  text-align: right;
  margin-top: -5px;
  font-weight: 700;
  font-size: 15px;
}
.pat_box i{
  color: #fd5621!important;
  font-size: 40px;
  padding: 3px;
  background: #e4e4e4;
  margin-left: 5px;
}
.box_marca{
  padding: 20px;
}
.img_testimoneo{
  border-radius: 50%;
  margin-top: -10px;
}
.title_testimoneo{
  font-style: italic;
  font-size: 15px;
  font-weight: 400;
}
.title_testimoneo_2{
  font-size: 13px;
}
@media (max-width: 550px){
  .img_testimoneo{
    width: 100px;
  }
  .title_testimoneo, .title_testimoneo_2 {
    text-align: center;
  }
}
</style>
