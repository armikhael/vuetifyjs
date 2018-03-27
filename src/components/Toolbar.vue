<template lang="html">

  <div>
    <v-toolbar app :clipped-left="clipped">
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
    </v-navigation-drawer>
  </div>

</template>

<script>
export default {
  data () {
    return {
      right: true,
      rightDrawer: false,
      clipped: false,
      fixed: false,
      items: [
        { title: 'Click Me' },
        { title: 'Click Me' },
        { title: 'Click Me' },
        { title: 'Click Me 2222222' }
      ]
    }
  }
}
</script>

<style scoped>
</style>
