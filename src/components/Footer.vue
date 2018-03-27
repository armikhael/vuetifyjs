<template lang="html">
  <div>
    <hr>
      <p>Footer</p>
    <hr>
    <v-footer class="footer_pharol">
      <v-container>
        <v-layout class="footer_row_resposive" row wrap>
          <v-flex xs12 sm4 md4>
            <br>
            <h3 class="title_footer">Newsletter</h3>
            <hr class="hr_footer">
            <br>
            <div class="input-group">
              <input type="text" class="form-control footer_email" placeholder="Tu email">
              <span class="input-group-addon"><i class="material-icons">&#xE163;</i></span>
            </div>
            <br>
            <p class="title_footer_2">"Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
            <p class="title_footer_3"><i class="material-icons">radio_button_unchecked</i> Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
            <br>
            <h3 class="title_footer">Redes</h3>
            <hr class="hr_footer">
            <br>
            <div class="footer_redes">
              <i class="material-icons color_gris">shopping_cart</i>
              <i class="material-icons color_gris">shopping_cart</i>
              <i class="material-icons color_gris">shopping_cart</i>
              <i class="material-icons color_gris">shopping_cart</i>
              <i class="material-icons color_gris">shopping_cart</i>
            </div>
          </v-flex>
          <v-flex xs12 sm3 md3>
            <br>
            <h3 class="title_footer">Contáctanos</h3>
            <hr class="hr_footer">
            <br>
            <p class="title_footer_3"><i class="material-icons footer_azul">person_pin</i> Dirección</p>
            <p class="title_footer_3">Lorem ipsum dolor sit<br> amet, consectetur adipiscing elit</p>
            <br>
            <p class="title_footer_3"><i class="material-icons footer_azul">person_pin</i> Teléfono / WhatsApp </p>
            <p class="title_footer_3">+00-000-0000 / +00-000-0000</p>
            <br>
            <p class="title_footer_3"><i class="material-icons footer_azul">person_pin</i> Email</p>
            <p class="title_footer_3">ejemplo@pharol.cl</p>
          </v-flex>
          <v-flex xs12 sm2 md2>
            <br>
            <h3 class="title_footer">Nosotros</h3>
            <hr class="hr_footer">
            <br>
            <div class="footer_nosotros">
              <p class="title_footer_3">Quienes somos</p>
              <p class="title_footer_3">Que es Pharol</p>
              <p class="title_footer_3">Misión y Visión</p>
              <p class="title_footer_3">Mapa del sitio</p>
              <p class="title_footer_3">Terminos y condiciones</p>
              <p class="title_footer_3">Políticas de privacidad</p>
              <p class="title_footer_3">Envios</p>
            </div>
          </v-flex>
          <v-flex xs12 sm3 md3>
            <br>
            <h3 class="title_footer">App</h3>
            <hr class="hr_footer">
            <br>
            <img class="resposive_img" src="@/assets/android.png">
            <img class="resposive_img" src="@/assets/apple.png">
            <br>
            <h3 class="title_footer">Medios de pago</h3>
            <hr class="hr_footer">
            <br>
            <img class="resposive_img" src="@/assets/webpage.png">
            <br>
            <h3 class="title_footer">Navegación Segura</h3>
            <hr class="hr_footer">
            <br>
            <img class="resposive_img" src="@/assets/seguro.png">
          </v-flex>
        </v-layout>
        <v-layout row>
          <v-flex xs12 class="footer_proy">
            <br>
            <h3 class="title_footer">Proyecto aprobado por</h3>
            <br>
            <img class="resposive_img" src="@/assets/inu.png">
          </v-flex>
        </v-layout>
      </v-container>
    </v-footer>
    <div class="footer_bottom">
      <p class="title_footer_2">"Copyright Pharol 2018 @ Derechos reservados</p>
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


<style scoped>

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
  margin-bottom: 0px;
  padding-bottom: 10px;
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
}

</style>
