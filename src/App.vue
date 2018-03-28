<template>
  <v-app>

    <component-toolbar></component-toolbar>

    <v-content>
        <component-product-detail> </component-product-detail>
        <component-slider></component-slider>
        <component-tabs></component-tabs>
        <component-tabs2></component-tabs2>
        <component-patologia></component-patologia>
    </v-content>
    <component-footer></component-footer>


  </v-app>
</template>

<script>
import Toolbar from './components/Toolbar'
import ProductDetail from './components/ProductDetail'
import Footer from './components/Footer'
import Tabs from './components/Tabs'
import Tabs2 from './components/Tabs2'
import Slider from './components/Slider'
import Patologia from './components/Patologia'

export default {
  name: 'App',
  components: {
    'component-toolbar': Toolbar,
    'component-product-detail': ProductDetail,
    'component-footer': Footer,
    'component-tabs': Tabs,
    'component-slider': Slider,
    'component-tabs2': Tabs2,
    'component-patologia': Patologia
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
.p10{
  padding: 10px;
}
.prl50{
  padding-left: 50px;
  padding-right: 50px;
}
.section-a{
  padding: 50px 0px;
  background: #f8f8f8;
}
.section-b{
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
.center{
  text-align: center;
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
  padding: 10px;
}
.detail_btn_add i{
  font-size: 16px;
  margin-left: 6px;
  margin-right: -10px;
}
.detail_btn_add {
  color: #fff!important;
  text-transform: none;
  margin-top: 15px;
  font-size: 12px;
  padding-left: 10px;
  padding-right: 10px;
}
.line_add_cart{
  color: #d6491c;
  padding-left: 10px;
  padding-right: 5px;
}


/*responsive 550*/
@media (max-width: 550px){
  .row_resposive{
    text-align: center;
  }
}
</style>
