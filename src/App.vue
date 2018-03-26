<template>
  <v-app>
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

    <v-content>
      <div class="">


      </div>
    </v-content>

    <v-navigation-drawer
      temporary
      :right="right"
      v-model="rightDrawer"
      fixed
      app
    >
    </v-navigation-drawer>

    <hr>
      Stepeer
    <hr>
    <v-stepper v-model="e1">
      <v-stepper-header>
        <v-stepper-step step="1" :complete="e1 > 1">Name of step 1</v-stepper-step>
        <v-divider></v-divider>
        <v-stepper-step step="2" :complete="e1 > 2">Name of step 2</v-stepper-step>
        <v-divider></v-divider>
        <v-stepper-step step="3">Name of step 3</v-stepper-step>
      </v-stepper-header>
      <v-stepper-items>
        <v-stepper-content step="1">
          <v-card color="grey lighten-1" class="mb-5" height="200px"></v-card>
          <v-btn color="primary" @click.native="e1 = 2">Continue</v-btn>
          <v-btn flat>Cancel</v-btn>
        </v-stepper-content>
        <v-stepper-content step="2">
          <v-card color="grey lighten-1" class="mb-5" height="200px"></v-card>
          <v-btn color="primary" @click.native="e1 = 3">Continue</v-btn>
          <v-btn flat>Cancel</v-btn>
        </v-stepper-content>
        <v-stepper-content step="3">
          <v-card color="grey lighten-1" class="mb-5" height="200px"></v-card>
          <v-btn color="primary" @click.native="e1 = 1">Continue</v-btn>
          <v-btn flat>Cancel</v-btn>
        </v-stepper-content>
      </v-stepper-items>
    </v-stepper>



    <hr>
      <p>Detalle del producto</p>
    <hr>
    <v-layout row>
      <v-flex x12 sm6 md6>
        <img src="http://www.nestle-family.com/uploads/product/6f46a57790ca4a3990a338f530685c7e.png" width="100%">
      </v-flex>
      <v-flex x12 sm6 md6>
        <v-text-field
          label="Label Text"
          type="number"
        ></v-text-field>
        <v-btn color="success">Success</v-btn>
      </v-flex>

    </v-layout>
    <v-layout row>
      <v-tabs
        v-model="active"
        color="cyan"
        dark
        slider-color="yellow"
        centered>
        <v-tab
          v-for="n in 3"
          :key="n"
          ripple>
          Item {{ n }}
        </v-tab>
        <v-tab-item
          v-for="n in 3"
          :key="n">
          <v-card flat>
            <v-card-text>{{ text }}</v-card-text>
          </v-card>
        </v-tab-item>
      </v-tabs>
    </v-layout>

    <hr>
      <p>Carousel de productos</p>
    <hr>

    <v-layout row>
      <v-carousel>
        <v-carousel-item>
          <v-layout row>
            <v-flex x12 sm3 md3>
              <v-card>
                <v-card-media src="http://www.nestle-family.com/uploads/product/6f46a57790ca4a3990a338f530685c7e.png" height="200px">
                </v-card-media>
                <v-card-title primary-title>
                  <div>
                    <h3 class="headline mb-0">Kangaroo Valley Safari</h3>
                    <div>Located two hours south of Sydney in the <br>Southern Highlands of New South Wales, ...</div>
                  </div>
                </v-card-title>
                <v-card-actions>
                  <v-btn flat color="orange">Share</v-btn>
                  <v-btn flat color="orange">Explore</v-btn>
                </v-card-actions>
              </v-card>
            </v-flex>
            <v-flex x12 sm3 md3>
              <v-card>
                <v-card-media src="http://www.nestle-family.com/uploads/product/6f46a57790ca4a3990a338f530685c7e.png" height="200px">
                </v-card-media>
                <v-card-title primary-title>
                  <div>
                    <h3 class="headline mb-0">Kangaroo Valley Safari</h3>
                    <div>Located two hours south of Sydney in the <br>Southern Highlands of New South Wales, ...</div>
                  </div>
                </v-card-title>
                <v-card-actions>
                  <v-btn flat color="orange">Share</v-btn>
                  <v-btn flat color="orange">Explore</v-btn>
                </v-card-actions>
              </v-card>
            </v-flex>
            <v-flex x12 sm3 md3>
              <v-card>
                <v-card-media src="http://www.nestle-family.com/uploads/product/6f46a57790ca4a3990a338f530685c7e.png" height="200px">
                </v-card-media>
                <v-card-title primary-title>
                  <div>
                    <h3 class="headline mb-0">Kangaroo Valley Safari</h3>
                    <div>Located two hours south of Sydney in the <br>Southern Highlands of New South Wales, ...</div>
                  </div>
                </v-card-title>
                <v-card-actions>
                  <v-btn flat color="orange">Share</v-btn>
                  <v-btn flat color="orange">Explore</v-btn>
                </v-card-actions>
              </v-card>
            </v-flex>
            <v-flex x12 sm3 md3>
              <v-card>
                <v-card-media src="http://www.nestle-family.com/uploads/product/6f46a57790ca4a3990a338f530685c7e.png" height="200px">
                </v-card-media>
                <v-card-title primary-title>
                  <div>
                    <h3 class="headline mb-0">Kangaroo Valley Safari</h3>
                    <div>Located two hours south of Sydney in the <br>Southern Highlands of New South Wales, ...</div>
                  </div>
                </v-card-title>
                <v-card-actions>
                  <v-btn flat color="orange">Share</v-btn>
                  <v-btn flat color="orange">Explore</v-btn>
                </v-card-actions>
              </v-card>
            </v-flex>
          </v-layout>
        </v-carousel-item>
        <v-carousel-item>
          <v-layout row>
            <v-flex x12 sm3 md3>
              <v-card>
                <v-card-media src="http://www.nestle-family.com/uploads/product/6f46a57790ca4a3990a338f530685c7e.png" height="200px">
                </v-card-media>
                <v-card-title primary-title>
                  <div>
                    <h3 class="headline mb-0">Kangaroo Valley Safari</h3>
                    <div>Located two hours south of Sydney in the <br>Southern Highlands of New South Wales, ...</div>
                  </div>
                </v-card-title>
                <v-card-actions>
                  <v-btn flat color="orange">Share</v-btn>
                  <v-btn flat color="orange">Explore</v-btn>
                </v-card-actions>
              </v-card>
            </v-flex>
            <v-flex x12 sm3 md3>
              <v-card>
                <v-card-media src="http://www.nestle-family.com/uploads/product/6f46a57790ca4a3990a338f530685c7e.png" height="200px">
                </v-card-media>
                <v-card-title primary-title>
                  <div>
                    <h3 class="headline mb-0">Kangaroo Valley Safari</h3>
                    <div>Located two hours south of Sydney in the <br>Southern Highlands of New South Wales, ...</div>
                  </div>
                </v-card-title>
                <v-card-actions>
                  <v-btn flat color="orange">Share</v-btn>
                  <v-btn flat color="orange">Explore</v-btn>
                </v-card-actions>
              </v-card>
            </v-flex>
            <v-flex x12 sm3 md3>
              <v-card>
                <v-card-media src="http://www.nestle-family.com/uploads/product/6f46a57790ca4a3990a338f530685c7e.png" height="200px">
                </v-card-media>
                <v-card-title primary-title>
                  <div>
                    <h3 class="headline mb-0">Kangaroo Valley Safari</h3>
                    <div>Located two hours south of Sydney in the <br>Southern Highlands of New South Wales, ...</div>
                  </div>
                </v-card-title>
                <v-card-actions>
                  <v-btn flat color="orange">Share</v-btn>
                  <v-btn flat color="orange">Explore</v-btn>
                </v-card-actions>
              </v-card>
            </v-flex>
            <v-flex x12 sm3 md3>
              <v-card>
                <v-card-media src="http://www.nestle-family.com/uploads/product/6f46a57790ca4a3990a338f530685c7e.png" height="200px">
                </v-card-media>
                <v-card-title primary-title>
                  <div>
                    <h3 class="headline mb-0">Kangaroo Valley Safari</h3>
                    <div>Located two hours south of Sydney in the <br>Southern Highlands of New South Wales, ...</div>
                  </div>
                </v-card-title>
                <v-card-actions>
                  <v-btn flat color="orange">Share</v-btn>
                  <v-btn flat color="orange">Explore</v-btn>
                </v-card-actions>
              </v-card>
            </v-flex>
          </v-layout>
        </v-carousel-item>
      </v-carousel>
    </v-layout>



    <hr>
      <p>Footer</p>
    <hr>
    <v-footer class="footer_pharol">
      <v-container>
        <v-layout row wrap>
          <v-flex xs12 sm4 md4>
            <br>
            <h3 class="title_footer">Newsletter</h3>
            <hr class="hr_footer">
            <v-flex xs10 sm10 md10>
              <v-text-field
              label="Suscripcion"
              ></v-text-field>
            </v-flex>
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
  </v-app>
</template>

<script>
export default {
  name: 'App',
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
      ],

      /* DETALLE DEL PRODUCTO */
      active: null,
      text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.',

      /* STEPEER */
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
.menu_init_title{
  color: #212121;
  margin-top: 17px;
  text-transform: capitalize;
}
.menu_init_box{
  padding-right: 70px;
}

/*resposive img*/
.resposive_img{
  max-width: 100%;
}

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
</style>
