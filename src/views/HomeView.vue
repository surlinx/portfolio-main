<template>
  <v-app id="home">
    <NavBar />
    <v-container fluid>
      <div class="head">
        <v-row>
          <v-col cols="5">
            <div style="position: relative" class="mt-16">
              <h1 class="text-white">Hi</h1>
              <h1 class="text-white">I'm Renee</h1>
              <span class="text-white">preparatoriana</span><br />
              <v-btn tile dark class="text-white" variant="outlined"
                >Contactame</v-btn
              >
            </div>
          </v-col>
          <v-col cols="2">
            <div
              style="
                position: absolute;
                z-index: 9999;
                bottom: 0;
                margin-left: auto;
                margin-right: auto;
                left: 0;
                right: 0;
                text-align: center;
              "
            >
              <v-icon>fas fa-angle-double-down</v-icon>
            </div>
          </v-col>
          <v-col cols="5">
            <div style="position: relative; z-index: 9999" class="mt-16">
              <v-img
                src="../assets/renee-foto.jpeg"
                contain
                max-height="300"
              ></v-img>
            </div>
          </v-col>
        </v-row>
      </div>
      <v-col cols="12" class="mt-16" id="about">
        <div>
          <v-row>
            <v-col cols="12" sm="6">
              <div class="egg">
                <v-img src="../assets/renee.jpeg" max-height="300"></v-img>
              </div>
            </v-col>
            <v-col cols="12" sm="6">
              <h2 class="mt-16">About me</h2>
              <div style="width: 120px">
                <v-slider v-model="slider2" color="black" label=""> </v-slider>
              </div>
              <h4 class="mt-n4"> 2 años haciendo folklore</h4>
              <h4>Salsa,rock and roll,bachata etc</h4>
              <p class="text-grey">
                Experiencia intermedia en folklore con estados de la peninsula y Riviera maya; Salsa,bachata y Rock and Roll básico,
                tomando un curso en computación e inglés. Último año en la carrera de Administración de Recursos Humanos 
              </p>
              <v-btn tittle dark color="brown" class="mt-4">Descargar CV</v-btn>
              
            </v-col>
          </v-row>
        </div>
      </v-col>
      <div class="text-center mt-4">
        <h1>Lo que hago</h1>
        <div style="width: 120px; margin: 0 auto">
          <v-slider v-model="slider2" color="black" label=""></v-slider>
        </div>
      </div>
      <v-col cols="12" class="padd" id="portfolio">
        <div class="first" id="project">
          <v-row>
            <v-col cols="12">
              <div class="child">
                <v-btn
                  icon="fas fa-laptop"
                  color="brown"
                  class="text-white"
                ></v-btn>
                <h3 class="ml-3 mt-4">Web Desing</h3>
                <p class="text-grey ml-3 mt-4 text-caption">
                   <br />Tomo cursos en diseño Web los fines de semana en el colgeio CETEC<br />
                </p>
              </div>
              <div class="child">
                <v-btn
                  icon="fas fa-masks-theater"
                  color="brown"
                  class="text-white"
                ></v-btn>
                <h3 class="ml-3 mt-4">folklore</h3>
                <p class="text-grey ml-3 mt-4 text-caption">
                  <br />tome clases de folklore durante 2 años,tengo conocimiento en pasos básicos<br />
                </p>
              </div>
              <div class="child">
                <v-btn
                  icon="fas fa-dumbbell"
                  color="brown"
                  class="text-white"
                ></v-btn>
                <h3 class="ml-3 mt-4">pole sport</h3>
                <p class="text-grey ml-3 mt-4 text-caption">
                  actualmente nivel intermedio,conocimiento en figuras básicas e intermedias
                  <br />
                </p>
              </div>
            </v-col>
          </v-row>
          <v-divider></v-divider>
        </div>
      </v-col>
      <v-col cols="12" sm="12" id="services">
        <div class="d-flex justify-center mb-6">
          <v-btn color="brown" class="mr-2">Todos</v-btn>
          <v-btn class="mr-2" variant="tonal">pole sport</v-btn>
          <v-btn class="mr-2" variant="tonal">folklore</v-btn>
          <v-btn class="mr-2" variant="tonal">diseño grafico</v-btn>
          <v-btn class="mr-2" variant="tonal"
            >constancia en prevencion y atencion de violencia sexual contra la
            mujer</v-btn>
        </div>
      </v-col>
      <v-col cols="12" class="imHover">
        <v-row class="fill-height" align="center" justify="center">
          <template>
            <v-col cols="12" md="4" v-for="(item, i) in items" :key="i">
              <v-hover v-slot="{ isHovering, props }">
                <v-card
                  :elevation="isHovering ? 12 : 2"
                  :class="{ 'on-hover': isHovering }"
                  v-bind="props"
                >
                  <v-img :src="item.img" height="255px" cover></v-img>
                </v-card>
              </v-hover>
            </v-col>
          </template>
        </v-row>
      </v-col>
      <v-col cols="12" sm="12">
        <div class="d-flex justify-center mb-6">
          <v-btn color="brown" class="mt4"> Conocer más</v-btn>
        </div>
      </v-col>
      <v-col cols="12" id="page">
        <div class="pre">
          <v-row>
            <v-card class="mw-auto" maxwidth="344" height="">
              <v-img src="renee.jpeg" height="200px" cover></v-img>
              <v-card-title>Renee Jacquelinne Sulub Can</v-card-title>
              <v-card-sibtitle>Motivos por los cuales contratarme</v-card-sibtitle>
              <v-card-text>Disposición en aprender lo necesario para aplicar y ejercer el puesto indicado, 
                personalidad tranquila y amistosa lejos de buscar problemas o ser un individuo violento, trabajo en equipo y organización. Servicios en áreas adminsitrativas de contratación de personal.
              </v-card-text >
            </v-card>
          </v-row>
        </div>
      </v-col>
      <v-col cols="12" id="biog">
        <div class="hire">
          <v-row>
            <v-col cols="12" sm="8">

              <h1>contratame</h1>
              <p>
                nacida en 2007 cancún Q.Roo el dia 6 de octubre ,actualmente estudiante sin experiencia laboral, interesada en aprender;
                Formación acádemica en Cetmar PDC carrera en admón RRHH,
                 deportista artistica durante el tiempo libre, estúdio computo por lapsos descontinuos 2017-2017, 2019-2020, 2022-2024. 
              </p>
            </v-col>
            <v-col cols="12" sm="4">
              <v-btn color="brown" class="mt-15"> contratame</v-btn>
            </v-col>
          </v-row>
        </div>
      </v-col>
      <v-col cols="12" id="blog">
        <h1>Blog</h1>
      <v-col cols="12" sm="12" class="px-16" id="contact">
        <v-row>
          <v-col cols="12" sm="4">
            <div class="child">
              <h1>Información de contacto</h1>
              <v-btn
               icon="fas fa-square-phone"
               color="white"
               class="text-brown" 
               ></v-btn>
               <p class="text-grey ml-3 mt-4 text-overline"> cel:9841868801</p>

               <v-btn
               icon="fas fa-square-envelope"
               color="white"
               class="text-brown"
               ></v-btn><br>
               <p class=" text-grey ml-3 mt-4 text-overline">e-mail:rjsc6reneeo4@gmail.com </p>

                <v-btn
               icon="fas fa-building"
               color="white"
               class="text-brown"
               ></v-btn> <br>
               <h4 class=" text-grey ml-3 mt-4 text-overline"> Av. constituyentes edificio 3  </h4>
            </div>
          </v-col>
          <v-col cols="12" sm="8">
            <h1 class="mt-8"> Send your message here</h1>
            <v-divider></v-divider>
            <v-text-field label="Nombre"></v-text-field> <br>
            <v-text-field label="Telefono"></v-text-field> <br>
            <v-text-field label="Correo Electronico"></v-text-field> <br>
             <v-text-field label="Mensaje"></v-text-field> <br>
            <v-btn color="brown">Submit</v-btn>
          </v-col>
        </v-row>
        </v-col>
        </v-col>
       
    </v-container>
  </v-app>
</template>

<script>
import { defineComponent } from "vue";

// Components
import NavBar from "../components/NavBar.vue";

export default defineComponent({
  name: "HomeView",
  setup() {
    return {
      slider2: 50,
      items: [{ img: "renee-foto.jpeg" }],
    };
  },
  components: {
    NavBar,
  },
});
</script>

<style scoped>
.v-container {
  padding-top: 16px 0;
}
.head {
  position: relative;
  text-align: center;
  padding: 12px;
  margin-bottom: 6px;
  height: 400px;
  width: 100%;
  color: white;
}
.head:before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 50%;
  background: rgb(41, 23, 3);
  transform: skew(0deg, 6deg);
}
.head:after {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  height: 100%;
  width: 50%;
  background: rgb(41, 23, 3);
  transform: skew(0deg, -6deg);
}
.egg {
  display: block;
  margin-left: 100px;
  margin-top: 50px;
  width: 365px;
  height: 300px;
  background-color: #ebdbb9;
  border-radius: 50% 50% 50% 50% / 60% 60% 40% 0%;
}
.first {
  width: 100%;
  height: 280px;
  text-align: center;
  padding: 2rem 2rem;
}
.child {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: center;
  margin-right: 8px;
}
.imgHover {
  padding: 0 200px;
}
.pre {
  width: 100%;
  height: 380px;
  text-align: center;
  padding: 0 200px;
  background-color: burlywood;
}
.hire {
  width: 100%;
  height: 200px;
  padding: 0 200px;
  background-color: #e9e9e9;
  margin-top: -24px;
}
</style>
