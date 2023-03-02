<template>
  <v-container fluid>
      <welcome texto="AIRE ACONDICIONADO"/>
      <v-row align="center" justify="center">
          <v-col cols="12" md="10" sm="12"  align="center" justify="center">
              <v-row align="center" justify="center">
                  <v-col cols="12" sm="12" md="6"  v-for="(inf, index) in productos" :key="index">
                      <div>
                          <img :src="inf.src" width="60%"/>
                          <h1>{{ inf.nombre }}</h1>
                          <p class="DescripcionProductos">{{ inf.Descripcion }}</p>
                          <v-btn :to="inf.to">
                              Ver Más
                          </v-btn>
                      </div>
                  </v-col>
              </v-row>
          </v-col>
      </v-row>
  </v-container>
</template>
<script>
import welcome from '../welcome.vue'; 
export default {
  components: {  welcome },
  data() {
      return{
          //Aca se crea un arreglo con los productos
          productos:[
              {src: '../../img/productos/bateria_2.png', nombre:'MUST', Descripcion:'El controlador de carga Must Solar es el primer dispositivo que se de conectar a las baterías para garantizar la integridad del sistema, del mismo modo, el último dispositivo que se de desconectar del controlador de carga Must Solar son las baterías.'},
              {src: '../../img/productos/Calentador-Ele.png', nombre:'STECA', Descripcion:'Steca Solarix MPPT son controladores de carga solar con se- guimiento del punto de máxima potencia. Estos son adecuados para todas las tecnologías de módulos comunes y son ideales para sistemas solares con voltajes de módulo más altos que el voltaje de la batería.'},
              {src: '../../img/productos/controlador_de_carga.png', nombre:'SMART SOLAR', Descripcion:'El SmartSolar cuida de la salud de la batería, ampliando su vida útil. El controlador de carga SmartSolar recargará hasta una batería extremadamente agotada. Puede funcionar con una tensión de batería de hasta 0 voltios, siempre que las celdas no estén sulfatadas o dañadas de forma permanente.'},
              {src: '../../img/productos/inversor_2.png', nombre:'SRNE', Descripcion:'Los reguladores de carga SRNE son conocidos por su versatilidad y larga vida útil a un ajustado precio compitiendo con otras reconocidas marcas del mercado de reguladores de carga que ofrecen las mismas prestaciones a un precio más alto.'},
      ]     
      }

  },
}
</script>