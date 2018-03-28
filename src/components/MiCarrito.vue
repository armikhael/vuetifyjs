<template lang="html">
  <div>
    <h1>Mi carrito de compra</h1>
    <div class="box_cart_menu">
      <v-layout class="content_cart_menu">
        <div style="width:100px">
          <img src="@/assets/carrito.png" width="100%">
        </div>
        <v-flex xs12 sm10 sm10 class="p10">
          <h3 class="title_cart_menu_title_1">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</h3>
            <div class="detail_box_number_cart_menu">
              <h3 class="cart_manu_price">$ 99.20</h3>
              <div class="cart_menu_box_number">
                <v-btn fab dark small color="naranja">
                  <v-icon dark style="font-size:10px;    font-weight: bold;">remove</v-icon>
                </v-btn>
                <input type="text" placeholder="0" class="form-control detail_number_cart_menu">
                <v-btn fab dark small color="naranja">
                  <v-icon dark style="font-size:10px;    font-weight: bold;">add</v-icon>
                </v-btn>
                <a href="#" class="cart_menu_delete">
                  <i class="material-icons">delete</i>
                </a>
              </div>
            </div>
        </v-flex>
      </v-layout>
    </div>
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
  .box_cart_menu{
    padding: 10px;
  }
  .content_cart_menu{
    border-bottom: 1px solid #ddd;
  }
  .title_cart_menu_title_1{
    font-size: 12px;
    font-weight: 300;
    color: #757575;
    overflow: hidden;
    text-overflow: ellipsis;
    -webkit-line-clamp: 2;
    display: -webkit-box;
    -webkit-box-orient: vertical;
    margin-top: -5px;
  }
  .cart_manu_price{
    font-size: 22px;
  }
  .detail_box_number_cart_menu{
    padding-top: 5px;
  }
  .cart_menu_box_number{
    text-align: right;
    margin-top: -30px;
  }
  .detail_number_cart_menu{
    border: 1px solid #ddd;
    width: 27px;
    text-align: center;
    border-radius: 0px;
    margin-top: 2px;
  }
  .cart_menu_delete i{
    color: #757575;
    font-size: 15px;
    padding-left: 10px;
  }
  .detail_box_number_cart_menu button{
    height: 15px!important;
    width: 15px!important;
    margin-top: 0px;
  }
</style>
