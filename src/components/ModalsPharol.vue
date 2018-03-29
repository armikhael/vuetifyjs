<template lang="html">
  <div>
    <v-layout row justify-center>
     <v-btn color="primary" dark @click.native.stop="dialog = true">Open Dialog</v-btn>
     <v-dialog v-model="dialog" max-width="600">
       <v-card>
         <v-card-title class="headline tile_modals_pharol"><h3>Use Google's location service?</h3></v-card-title>
         <v-card-text class="tile_modals_pharol_2">Let Google help apps determine location. This means sending anonymous location data to Google, even when no apps are running.Let Google help apps determine location. This means sending anonymous location data to Google, even when no apps are running.</v-card-text>
         <div class="box_modals_input">
           <v-text-field
             label="Buscar Dirección"
             v-model="name"
             :rules="nameRules"
             required
           ></v-text-field>
         </div>
         <v-card-actions class="btn_box_modals_pharol">
           <v-spacer></v-spacer>
           <v-btn class="naranja btn_modals_pharol" @click.native="dialog = false">Aceptar</v-btn>
         </v-card-actions>
       </v-card>
     </v-dialog>
   </v-layout>
  </div>
</template>

<script>
export default {
    data () {
      return {
        dialog: false
      }
    }
  }
</script>

<style>
.btn_box_modals_pharol{
  text-align: center!important;
  display: block;
  padding: 20px;
}
.tile_modals_pharol{
  text-align: center!important;
  border-bottom: 3px solid #5e0093;
  background: #f9f9f9;
  box-shadow: 0 2px 2px -2px #5e0093;
}
.tile_modals_pharol h3{
  width: 100%;
  color: #5e0093;
  font-weight: 600;
  font-size: 20px;
}
.tile_modals_pharol_2{
  text-align: center;
  padding: 20px;
  color: #7c7c7c;
}
.btn_modals_pharol{
  color: #fff!important;
  text-transform: none;
  text-align: center;
}
.box_modals_input{
  padding: 0px 30px 0px 30px;
}
</style>
