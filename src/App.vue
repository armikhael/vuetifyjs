<template>
  <v-app>

    <component-toolbar></component-toolbar>
    <!-- <v-toolbar app :clipped-left="clipped">
      <img src="@/assets/logoapp.png" alt="Vuetify.js">
      <v-spacer></v-spacer>
      <v-menu left class="menu_init_box">
        <v-btn icon dark slot="activator">
          <i class="material-icons color_gris">person_pin</i> <p class="menu_init_title">Iniciar</p>
        </v-btn>
        <v-list>
          <v-list-tile v-for="(item, index) in items" :key="index" @click="">
            <v-list-tile-title>{{ item.title }}</v-list-tile-title>
          </v-list-tile>
        </v-list>
      </v-menu>
      <v-btn icon @click.stop="rightDrawer = !rightDrawer">
        <i class="material-icons color_gris">shopping_cart</i>
        <span class="badge__badge naranja">0</span>
      </v-btn>
    </v-toolbar>
    <v-navigation-drawer
      temporary
      :right="right"
      v-model="rightDrawer"
      fixed
      app
    >
    </v-navigation-drawer> -->

    <v-content>
        <component-product-detail> </component-product-detail>
        <component-tabs></component-tabs>
        <!-- <hr>
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
              <img class="resposive_img" src="@/assets/rr.png">
              <img class="resposive_img" src="@/assets/rr.png">
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
                 <v-card-title primary-title>
                   <div>
                     <h4 class="carru_title_1">Corcidin Gotas Pediatricas Caja con Frasco Con 30 ML Rx</h4>
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
        </v-layout> -->
    </v-content>


    <component-tabs-icon-text></component-tabs-icon-text>

    <component-footer></component-footer>


  </v-app>
</template>

<script>
import Toolbar from './components/Toolbar'
import ProductDetail from './components/ProductDetail'
import Footer from './components/Footer'
import Tabs from './components/Tabs'
import TabsIconText from './components/TabsIconText'

export default {
  name: 'App',
  components: {
    'component-toolbar': Toolbar,
    'component-product-detail': ProductDetail,
    'component-footer': Footer,
    'component-tabs': Tabs,
    'component-tabs-icon-text': TabsIconText

  },
  data () {
    return {
      e1: 0
    }
  }
}
</script>

<style>
.toolbar__content, .toolbar__extension {
  background: #fbfbfb;
}
.badge--left .badge__badge {
  left: -22px;
}

.badge__badge {
    color: #fff;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    position: absolute;
    top: -5px;
    right: -3px;
    border-radius: 50%;
    height: 18px;
    width: 18px;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
    -webkit-box-orient: horizontal;
    -webkit-box-direction: normal;
    -ms-flex-direction: row;
    flex-direction: row;
    -ms-flex-wrap: wrap;
    flex-wrap: wrap;
    -webkit-transition: .3s cubic-bezier(.25,.8,.5,1);
    transition: .3s cubic-bezier(.25,.8,.5,1);
}
.color_gris{
  color: #d4d4d4;
}
.menu_init_title{
  color: #212121;
  margin-top: 17px;
  text-transform: capitalize;
}
.menu_init_box{
  padding-right: 70px;}













/*General*/
.application.theme--light {
    background: #ffff;
    color: rgba(0,0,0,0.87);
}
.p50{
  padding: 50px;
}
.prl50{
  padding-left: 50px;
  padding-right: 50px;
}
.section-a{
  padding: 50px 0px;
  background: #f8f8f8;
}
.blue_app{
  background-color: #268ae0 !important;
  border-color: #268ae0 !important;
}
.naranja {
    background-color: #fd5621!important;
    border-color: #fd5621!important;
}


/*resposive img*/
.resposive_img{
  max-width: 100%;
}



/*Producto*/
.triangulo_equilatero {
     width: 0;
     height: 0;
     border-right: 40px solid transparent;
     border-top: 40px solid #f8002d;
     border-left: 40px solid #f8002d;
     border-bottom: 40px solid transparent;
}
.box_triangulo{
  position: absolute;
  top:0;
  left: 0px;
}
.triangulo_equilatero p{
  position: absolute;
  top: 0;
  left: 0;
  padding: 12px;
  color: #fff;
  font-weight: 900;
}
.carru_add_cart_btn{
  text-align: center;
  padding-bottom: 15px;
}
.carru_title_1{
  color: blue;
  font-size: 13px;
}
.carru_title_2{
  color: #9a9a9a;
  font-size: 12px;
  margin-top: 5px;
  margin-bottom: 10px;
}
.carru_title_3{
  color: #f8002d;
  font-size: 15px;
}
.carru_title_4{
  color: #9a9a9a;
  font-size: 12px;
  text-decoration:line-through;
}
.product-overlay {
    background: #ffffff80;
    top: 0;
    display: none;
    height: 0;
    position: absolute;
    -webkit-transition: height 500ms ease 0s;
    transition: height 500ms ease 0s;
    width: 100%;
    display: block;
}
.product-overlay .overlay-content {
    position: absolute;
    bottom: 0;
    text-align: center;
    width: 100%;
}
.product-overlay h2 {
    color: #212121;
    font-family: 'Roboto', sans-serif;
    font-size: 12px;
    font-weight: 700;
}
.product-overlay p {
    font-family: 'Roboto', sans-serif;
    font-size: 10px;
    font-weight: 400;
    color: #212121;
}
.product-overlay .add-to-cart {
    background: #fff;
    border: 0 none;
    border-radius: 0;
    color: #FE980F;
    font-family: 'Roboto', sans-serif;
    font-size: 15px;
    margin-bottom: 25px;
}
.add-to-cart i {
    margin-right: 5px;
}

.single-products:hover .product-overlay {
    display: block;
    height: 100%;
}
.single-products {
    position: relative;
}

.product-image-wrapper {
    overflow: hidden;
}
.product_box_hover{
  padding: 15px;
}


/*responsive 550*/
@media (max-width: 550px){
  .row_resposive{
    text-align: center;
  }
}
</style>
