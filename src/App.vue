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
    <component-footer></component-footer>


  </v-app>
</template>

<script>
import Toolbar from './components/Toolbar'
import ProductDetail from './components/ProductDetail'
import Footer from './components/Footer'

export default {
  name: 'App',
  components: {
    'component-toolbar': Toolbar,
    'component-product-detail': ProductDetail,
    'component-footer': Footer
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
.naranja {
    background-color: #fd5621!important;
    border-color: #fd5621!important;
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
  padding-right: 70px;

/*General*/
}.application.theme--light {
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

/*resposive img*/
.resposive_img{
  max-width: 100%;
}

/*Footer*/
.footer_pharol{
  background: #161616!important;
  height: auto!important;
}
.title_footer{
  color: #fff;
  font-size: 14px;
}
.hr_footer{
  margin-top: 10px;
  margin-bottom: 10px;
  width: 70px;
  border: 1px solid #268ae0;
}
.title_footer_2{
  color: #fff;
}
.title_footer_3{
  color: #fff;
  font-size: 12px;
}
.title_footer_3 i{
  font-size: 13px;
  font-weight: 900;
  padding-right: 5px;
}
.footer_redes i{
  font-size: 40px;
  padding-right: 10px;
}
.footer_azul{
  color: #268ae0;
}
.footer_proy{
  text-align: center;
}
.footer_bottom{
  text-align: center;
  background: #02050c;
  padding-top: 10px;
}
.input-group {
    position: relative;
    display: -webkit-box;
    display: -webkit-flex;
    display: -ms-flexbox;
    display: flex;
    width: 100%;
}
.form-control {
    display: block;
    width: 100%;
    padding: .5rem .75rem;
    font-size: 1rem;
    line-height: 1.25;
    color: #464a4c;
    background-color: #fff;
    background-image: none;
    -webkit-background-clip: padding-box;
    background-clip: padding-box;
    border: 0px solid rgba(0,0,0,.15);
    border-radius: .25rem;
    -webkit-transition: border-color ease-in-out .15s,-webkit-box-shadow ease-in-out .15s;
    transition: border-color ease-in-out .15s,-webkit-box-shadow ease-in-out .15s;
    -o-transition: border-color ease-in-out .15s,box-shadow ease-in-out .15s;
    transition: border-color ease-in-out .15s,box-shadow ease-in-out .15s;
    transition: border-color ease-in-out .15s,box-shadow ease-in-out .15s,-webkit-box-shadow ease-in-out .15s;
}
.input-group-addon {
    padding: .5rem .75rem;
    margin-bottom: 0;
    font-size: 1rem;
    font-weight: 400;
    line-height: 1.25;
    color: #fff;
    text-align: center;
    background-color: #268ae0;

    border-radius: 0px 2px 2px 0px;
}
.footer_email{
    width: 75%!important;
    border-radius: 2px 0px 0px 2px;
}
/*Detail Producto*/
.menu_history{
  color: #8e8e8e;
  font-size: 12px;
}
.detail_img_product{
  text-align: center;
}
.detail_img_product img{
  width: 100%;
}
.detail_title2{
  margin-bottom: 5px;
  color: #8e8e8e;
  font-size: 13px;
}
.detail_hr{
  border: 1px solid #ddd;
}
.detail_number{
  border: 1px solid #ddd;
  width: 40px;
  text-align: center;
  border-radius: 0px;
  margin-top: 2px;
}
.detail_box_number{
  display: -webkit-box;
  margin-top: 15px;
}
.btn--floating.btn--small {
    height: 30px;
    width: 30px;
}
.detail_btn_add{
  color: #fff!important;
  text-transform: capitalize;
  margin-top: 15px;
}
.detail_redes i{
  font-size: 25px;
  padding-right: 10px;
  color: #212121;
}
.detail_tabs{
  width: 100%;
}
.detail_title_tabs{
  color: #212121!important;
}
.tabs__container{
  border-bottom: 1px solid #f9f7f7;
}

/*responsive 768*/
@media (min-width: 768px){
  .detail_img_product img{
    width: 300px;
  }
  .detail_product_caract{
    border-left:    2px solid #e0e0e0;
  }

}

/*responsive 550*/
@media (max-width: 550px){
  .footer_row_resposive{
    text-align: center;
  }
  .hr_footer {
    margin: 0 auto;
  }
  .title_footer {
    margin-bottom: 15px;
  }
  .footer_email{
      width: 100%;
    }
  .hr_detail{
    display: none;
  }
  .row_resposive{
    text-align: center;
  }
    .detail_box_number {
      display: block;
  }
  .detail_number{
    margin: 0 auto;
  }
}
</style>
