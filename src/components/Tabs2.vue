<template lang="html">
  <v-layout row>
    <v-tabs class="detail_container_tabs"
      v-model="active"
      color="white"
      dark
      slider-color="blue_app"
      centered>
      <v-tab class="detail_title_tabs_2"
        v-for="n in 4"
        :key="n"
        ripple>
        <i class="material-icons color_gris">shopping_cart</i>
        <h4 class="title_tabs2">Item {{ n }}</h4>
      </v-tab>
      <v-tab-item
        v-for="n in 4"
        :key="n">
        <v-card flat class="card_tabs2">
          <v-card-text>{{ text }}</v-card-text>
        </v-card>
      </v-tab-item>
    </v-tabs>
  </v-layout>
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
.detail_title_tabs_2{
  color: #8a8a8a!important;
}
.tabs__slider {
    display: none;
}
.detail_title_tabs_2 a{
  display: block;
}
.title_tabs2{
  text-transform: capitalize;
}
.tabs__item{
  padding-top: 20px;
}
.tabs__item i{
  font-size: 30px;
  margin-bottom: 10px;
}
.tabs__item--active i{
  color: #268ae0;
}
.tabs__item--active{
  background: #e5e5e5;
  border-top: 2px solid #268ae0;
  padding-top: 20px;
  color: #212121!important;
}
.card_tabs2{
  background-color: #e5e5e5!important;
}
.tabs__container{
  height: 90px;
  border-bottom: 1px solid #999999;
}
</style>
