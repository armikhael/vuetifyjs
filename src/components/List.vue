<template lang="html">
  <div>
    <div class="box_card">
      <v-card class="box_card_2">
        <v-container>
          <div class="box_cart_list">
            <v-layout class="content_cart_list">
              <div style="width:100px">
                <img src="@/assets/carrito.png" width="100%">
              </div>
              <v-flex xs12 sm12 sm12 class="p10 center-res">
                <v-layout row wrap>
                  <v-flex xs12 sm6 sm6>
                    <h3 class="title_cart_list_title_1">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</h3>
                    <p class="title_cart_list_title_2">Laboratorio Chile</p>
                    <img class="resposive_img" width="44px" src="@/assets/rr.png">
                  </v-flex>
                  <v-flex xs12 sm2 sm2 class="center">
                    <h3 class="cart_list_price">$ 99.20</h3>
                  </v-flex>
                  <v-flex xs12 sm2 sm2 class="center">
                    <div class="cart_list_box_number">
                      <v-btn fab dark small color="naranja">
                        <v-icon dark style="font-size:15px;    font-weight: bold;">remove</v-icon>
                      </v-btn>
                      <input type="text" placeholder="0" class="form-control detail_number_cart_list">
                      <v-btn fab dark small color="naranja">
                        <v-icon dark style="font-size:15px;    font-weight: bold;">add</v-icon>
                      </v-btn>
                    </div>
                  </v-flex>
                  <v-flex xs12 sm2 sm2 class="center">
                    <v-btn class="cart_list_clear">
                      <i class="material-icons" style="color: #ff004c;font-size: 20px;">delete</i>
                    </v-btn>
                    <span class="line_list_cart">|</span>
                    <v-btn class="cart_list_clear">
                      <i class="material-icons" style="color: #08bdd6;font-size: 20px;">av_timer</i>
                    </v-btn>
                  </v-flex>
                </v-layout>
              </v-flex>
            </v-layout>
          </div>
        </v-container>
      </v-card>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      init: null
    }
  }
}
</script>

<style>
.box_card{
  padding: 20px;
}
.box_card_2{
  padding: 10px;
}
.box_cart_list{
  padding: 10px;
}
.content_cart_list{
  border-bottom: 1px solid #ddd;
}
.title_cart_list_title_1{
  font-size: 14px;
  font-weight: 300;
  color: #268ae0;
  overflow: hidden;
  text-overflow: ellipsis;
  -webkit-line-clamp: 2;
  display: -webkit-box;
  -webkit-box-orient: vertical;
}
.title_cart_list_title_2{
  font-size: 12px;
  color:#757575;
  margin-bottom: 5px;
}
.cart_list_price{
  font-size: 22px;
}
.detail_number_cart_list{
  border: 1px solid #ddd;
  width: 35px;
  text-align: center;
  border-radius: 0px;
  margin-top: 2px;
}
.cart_list_clear{
  box-shadow: none!important;
  background-color: transparent!important;
  min-width: 10px!important;
}
.line_list_cart{
  color: #ebebeb;
  padding-left: 0px;
  padding-right: 1px;
}
@media (max-width: 550px){
  .center-res{
    text-align: center;
  }
}
</style>
