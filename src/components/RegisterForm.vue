<template lang="html">
  <div>
    <div class="box_login">
      <v-card class="box_login_2">
        <v-container>
          <v-btn class="btn_redes_form"><img class="resposive_img" src="@/assets/facebook.png" width="26px"> Registrarse con Facebook</v-btn>
          <br>
          <v-btn class="btn_redes_form"><img class="resposive_img" src="@/assets/google.png" width="26px"> Registrarse con Google</v-btn>
          <br><br>
          <h3 class="title_form_register">O completa el siguiente formulario</h3>
          <br>
          <v-layout row wrap>
            <v-flex xs12 sm5 sm5 class="p10 mx-auto">
              <div class="input_group_form">
                <span class="input_group_addon_form"><i class="material-icons">&#xE163;</i></span>
                <input type="text" class="form_control form_register_input_2" placeholder="Nombre">
                <span class="requerido_form">*</span>
              </div>
            </v-flex>
            <v-flex xs12 sm5 sm5 class="p10 mx-auto">
              <div class="input_group_form">
                <span class="input_group_addon_form"><i class="material-icons">&#xE163;</i></span>
                <input type="text" class="form_control form_register_input_2" placeholder="Apellido">
                <span class="requerido_form">*</span>
              </div>
            </v-flex>
          </v-layout>
          <br>
          <v-layout row wrap>
            <v-flex xs12 sm5 sm5 class="p10 mx-auto">
              <div class="input_group_form">
                <span class="input_group_addon_form"><i class="material-icons">&#xE163;</i></span>
                <input type="text" class="form_control form_register_input_2" placeholder="E-mail">
                <span class="requerido_form">*</span>
              </div>
            </v-flex>
            <v-flex xs12 sm5 sm5 class="p10 mx-auto">
              <div class="input_group_form">
                <span class="input_group_addon_form"><i class="material-icons">&#xE163;</i></span>
                <input type="text" class="form_control form_register_input_2" placeholder="Confirmar E-mail">
                <span class="requerido_form">*</span>
              </div>
            </v-flex>
          </v-layout>
          <br>
          <v-layout row wrap>
            <v-flex xs12 sm5 sm5 class="p10 mx-auto">
              <div class="input_group_form">
                <span class="input_group_addon_form"><i class="material-icons">&#xE163;</i></span>
                <input type="text" class="form_control form_register_input_2" placeholder="Contraseña">
                <span class="requerido_form">*</span>
              </div>
            </v-flex>
            <v-flex xs12 sm5 sm5 class="p10 mx-auto">
              <div class="input_group_form">
                <span class="input_group_addon_form"><i class="material-icons">&#xE163;</i></span>
                <input type="text" class="form_control form_register_input_2" placeholder="Confirmar contraseña">
                <span class="requerido_form">*</span>
              </div>
            </v-flex>
          </v-layout>
          <br>
          <v-layout row wrap>
            <v-flex xs12 sm5 sm5 class="p10 mx-auto">
              <div class="input_group_form">
                <span class="input_group_addon_form"><i class="material-icons">&#xE163;</i></span>
                <input type="text" class="form_control form_register_input_2" placeholder="RUT">
              </div>
              <p class="rut_reque">"Lorem ipsum dolor sit amet, consectetur adipiscing elit radio_button_unchecked<br> Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
            </v-flex>
            <v-flex xs12 sm5 sm5 class="p10 mx-auto">
              <div class="input_group_form">
                <span class="input_group_addon_form"><i class="material-icons">&#xE163;</i></span>
                <input type="text" class="form_control form_register_input_2" placeholder="Telefono">
              </div>
            </v-flex>
          </v-layout>
          <br><br>
          <v-btn color="naranja detail_btn_register">Registrarse</v-btn>
          <br><br>
          <h3 class="form_cap_obli_text"><span class="requerido_form">*</span> Campos Obligatorios</h3>
          <v-checkbox label="Acepto" v-model="checkbox" required></v-checkbox>
        </v-container>
      </v-card>
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
.box_login{
  padding: 20px;
}
.box_login_2{
  padding: 10px;
  text-align: center;
}
.btn_redes_form{
  background: #fff!important;
  text-transform: none;
}
.btn_redes_form{
  font-weight: 400;
  font-size: 13px;
  width: 280px;
  height: 40px;
}
.btn_redes_form img{
  margin-right: 15px;
}
.title_form_register{
  font-size: 14px;
  padding-top: 20px;
}
.ml-auto, .mx-auto {
    margin-left: auto!important;
}
.mr-auto, .mx-auto {
    margin-right: auto!important;
}

.input_group_form {
    position: relative;
    display: -webkit-box;
    display: -webkit-flex;
    display: -ms-flexbox;
    display: flex;
    padding: 0!important;
    width: 100%;
}
.form_control {
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
    border: 1px solid #d8d8d8;
    border-radius: 2px;
    height: 42px;
    background: #f9f9f9;
}
.input_group_addon_form {
    padding: 3px 5px 5px 11px;
    margin-bottom: 0;
    font-size: 1rem;
    font-weight: 400;
    line-height: 1.25;
    color: #bbbbbb;
    text-align: center;
    background-color: #ededee;
    border-top: 1px solid #d8d8d8;
    border-bottom: 1px solid #d8d8d8;
    border-left: 1px solid #d8d8d8;
    border-radius: 2px 0px 0px 2px
}
.input_group_addon_form i{
  margin-top: 5px;
}
.form_register_input_2{
    width: 75%!important;
    border-radius: 0px 2px 2px 0px;
}
.requerido_form{
  color: red;
  margin-left: 15px;
}
.rut_reque{
  text-align: left;
  margin-top: 10px;
  font-size: 11px;
  font-weight: 200;
}
.detail_btn_register{
  text-transform: none;
  color:#fff!important;
  font-size: 15px!important;
  width: 250px;
}
.form_cap_obli_text{
  text-align: left;
  font-size: 14px;
  font-weight: 300;
}

@media (max-width: 550px){
  .form_register_input_2{
      width: 100%!important;
      border-radius: 0px 2px 2px 0px;
  }
}
</style>
