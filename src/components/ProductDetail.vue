<template lang="html">
  <div>
    <hr>
      <p>Detalle del producto</p>
    <hr>
    <v-container>
      <v-layout row wrap>
        <v-flex xs12 sm12 md12>
        <p class="menu_history">Inicio > Medicamentos > Tos y Gripa > Corcidin Gotas Pediatricas Caja con Frasco Con 30 ML Rx</p>
        </v-flex>
      </v-layout>
      <v-layout row wrap>
        <v-flex xs12 sm6 md6 class="p50">
          <div class="detail_img_product">
            <img class="resposive_img" src="@/assets/producto.png" width="100%">
          </div>
        </v-flex>
        <v-flex xs12 sm6 md6 class="detail_product_caract prl50 row_resposive">
          <h3>Corcidin Gotas Pediatricas Caja con Frasco Con 30 ML Rx</h3>
          <br>
          <p class="detail_title2">Princio(s) Activo(s)</p>
          <p class="detail_title2">Laboratorio Chile</p>
          <img class="resposive_img" width="44px" src="@/assets/rr.png">
          <img class="resposive_img" width="44px" src="@/assets/rr.png">
          <hr class="detail_hr">
          <br>
          <h2>$ 32.100</h2>
          <div class="detail_box_number">
            <v-btn fab dark small color="naranja">
              <v-icon dark>remove</v-icon>
            </v-btn>
            <input type="text" placeholder="0" class="form-control detail_number">
            <v-btn fab dark small color="naranja">
              <v-icon dark>add</v-icon>
            </v-btn>
          </div>
          <v-btn color="naranja detail_btn_add">Agregar al carro | <i class="material-icons">shopping_cart</i></v-btn>
          <br><br>
          <div class="detail_redes">
            <i class="material-icons color_gris">shopping_cart</i>
            <i class="material-icons color_gris">shopping_cart</i>
            <i class="material-icons color_gris">shopping_cart</i>
            <i class="material-icons color_gris">shopping_cart</i>
            <i class="material-icons color_gris">shopping_cart</i>
          </div>
        </v-flex>
      </v-layout>
    </v-container>
    <section class="section-a">
      <v-container>
        <v-layout>
         <v-flex xs12 sm3 sm3>
           <v-card>
             <a href="#">
               <div class="product-image-wrapper">
                 <div class="single-products">
                   <div class="box_triangulo">
                     <div class="triangulo_equilatero"><p>-31%</p></div>
                   </div>
                   <img class="resposive_img" src="@/assets/producto.png" width="100%">
                   <div class="product-overlay">
                     <div class="overlay-content">
                       <div class="product_box_hover">
                         <img class="resposive_img" src="@/assets/prot.png">
                         <h2>Este producto requiere receta cheque</h2>
                         <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                       </div>
                       <div class="product_box_hover">
                         <img class="resposive_img" src="@/assets/prot.png">
                         <h2>Este producto requiere receta cheque</h2>
                         <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                       </div>
                     </div>
                   </div>
                 </div>
               </div>
             </a>
             <v-card-title primary-title>
               <div>
                 <a href="#"><h4 class="carru_title_1">Corcidin Gotas Pediatricas Caja con Frasco Con 30 ML Rx</h4></a>
                 <p class="carru_title_2">Laboratorio Chile</p>
                 <h4 class="carru_title_3">$ 32.100 <span class="carru_title_4">$10.698</span></h4>
               </div>
             </v-card-title>
             <div class="carru_add_cart_btn">
               <v-btn color="naranja detail_btn_add">Agregar al carro | <i class="material-icons">shopping_cart</i></v-btn>
             </div>
           </v-card>
         </v-flex>
       </v-layout>
     </v-container>

    </section>

    <v-layout row>
      <v-tabs class="detail_container_tabs"
        v-model="active"
        color="white"
        dark
        slider-color="blue_app"
        centered>
        <v-tab class="detail_title_tabs"
          v-for="n in 4"
          :key="n"
          ripple>
          Item {{ n }}
        </v-tab>
        <v-tab-item
          v-for="n in 4"
          :key="n">
          <v-card flat>
            <v-card-text>{{ text }}</v-card-text>
          </v-card>
        </v-tab-item>
      </v-tabs>
    </v-layout>
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


<style scoped>
a:link {
    text-decoration: none!important;
}
</style>
