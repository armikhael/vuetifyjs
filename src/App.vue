<template>
  <v-app>
    <v-toolbar
      app
      :clipped-left="clipped"
    >
      <img src="@/assets/logoapp.png" alt="Vuetify.js">
      <v-spacer></v-spacer>
      <v-btn icon>
        <i class="material-icons color_gris">person_pin</i>
      </v-btn>
      <v-btn icon @click.stop="rightDrawer = !rightDrawer">
        <i class="material-icons color_gris">shopping_cart</i>
        <span class="badge__badge naranja">0</span>
      </v-btn>
    </v-toolbar>

    <v-content>
      <router-view/>
    </v-content>

    <v-navigation-drawer
      temporary
      :right="right"
      v-model="rightDrawer"
      fixed
      app
    >
      <v-list>
        <!--<v-list-tile @click="right = !right">
          <v-list-tile-action>
            <v-icon>compare_arrows</v-icon>
          </v-list-tile-action>
          <v-list-tile-title>Switch drawer (click me)</v-list-tile-title>
        </v-list-tile>-->
      </v-list>
    </v-navigation-drawer>
    <v-footer :fixed="fixed" app>
      <span>&copy; 2017</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      right: true,
      rightDrawer: false
    }
  },
  name: 'App'
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
</style>
