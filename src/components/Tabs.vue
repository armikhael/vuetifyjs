<template lang="html">
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
.tabs__container{
  border-bottom: 1px solid #f9f7f7;
}
.detail_tabs{
  width: 100%;
}
.detail_title_tabs{
  color: #212121!important;
}
</style>
