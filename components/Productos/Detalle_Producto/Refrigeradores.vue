<template>
  <v-container fluid>
      <welcome texto="REFRIGERADORES SOLARES"/>
      <v-row align="center" justify="center">
          <v-col cols="12" md="10" sm="12"  align="center" justify="center">
              <v-row align="center" justify="center">
                  <v-col cols="12" sm="12" md="6"  v-for="(inf, index) in productos" :key="index">
                      <div>
                          <img :src="inf.src" width="200"/>
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
              {src: '../../img/productos/bateria_2.png', nombre:'DC REFRIGERADOR 12/24 VCD DE 150LT', Descripcion:'Panel solar – 2 unids Cable LAPPTHERM solar XLS 4MM – 20m Terminal LAPP hembra – 1 unid Terminal LAPP macho – 1 unid Bateria AGM sellada 12V/45A – 2 unid Controlador – 1 unid Nezvera / Refrigerador 210L ( 1.8 cu.ft) 12 /24V Características: Una de las principales características del refrigerador solar, es el gabinete súper aislado, con una capa de 11 centímetros de aislamiento con una cubierta de acero galvanizado en el exterior y aluminio en la parte interior. Cuenta también con un sistema que reduce la escarcha y la humedad, por lo que es de fácil mantenimiento. También es un refrigerador ecológico ya que no contiene CFCs, usa refrigerante R-134a, que no daña la capa de ozono, de gran estabilidad química y térmica y una baja toxicidad, además de no ser inflamable.'},
              {src: '../../img/productos/Calentador-Ele.png', nombre:'DC REFRIGERADOR 12/24 VCD DE 258LT', Descripcion:'Panel solar 195Wp – 24VDC -- 2 unid Cable LAPPTHERM Solar XLS 4MM -- 20 unid Terminal LAPP hembra – 1 unid Terminal LAPP macho – 1 unid Bateria AGM sellada 12V/155A – 1 unid- Controlador MPPT 20/10A, 250W / 12V – 500W / 24V -100VDC Nevera / Refrigerador 235L (8.1cu.ft) 12 / 24 – 1unid Características: Cuenta también con un sistema que reduce la escarcha y la humedad, por lo que es de fácil mantenimiento. También es un refrigerador ecológico ya que no contiene CFCs, usa refrigerante R-134a, que no daña la capa de ozono, de gran estabilidad química y térmica y una baja toxicidad, además de no ser inflamable.'},
              {src: '../../img/productos/controlador_de_carga.png', nombre:'CONGELADOR SOLAR 100L', Descripcion:'Panel solar 180Wp – 12VDC - 2 unidCable LAPPTHERM Solar XLS 4MM - 20 unidTerminal LAPP hembra – 1 unidTerminal LAPP macho – 1 unidBateria AGM sellada 12V/75Ah – 2 unidControlador MPPT 20/10A, 250W/12V – 500W/24V – 1unidNevera- congelador solar 12/24V, 150L – 1 unid Características:Cuenta también con un sistema que reduce la escarcha y la humedad, por lo que es de fácil mantenimiento. También es un refrigerador ecológico ya que no contiene CFCs, usa refrigerante R-134a, que no daña la capa de ozono, de gran estabilidad química y térmica y una baja toxicidad, además de no ser inflamable. '},
              {src: '../../img/productos/inversor_2.png', nombre:'CONGELADOR SOLAR 150L', Descripcion:'Panel solar – 2 unids Cable LAPPTHERM solar XLS 4MM – 20m Terminal LAPP hembra – 1 unid Terminal LAPP macho – 1 unid Bateria AGM sellada 12V/45A – 2 unid Controlador – 1 unid Nezvera / Refrigerador 210L ( 1.8 cu.ft) 12 /24V Características: Una de las principales características del refrigerador solar, es el gabinete súper aislado, con una capa de 11 centímetros de aislamiento con una cubierta de acero galvanizado en el exterior y aluminio en la parte interior. Cuenta también con un sistema que reduce la escarcha y la humedad, por lo que es de fácil mantenimiento. También es un refrigerador ecológico ya que no contiene CFCs, usa refrigerante R-134a, que no daña la capa de ozono, de gran estabilidad química y térmica y una baja toxicidad, además de no ser inflamable.'},
              {src: '../../img/productos/inversor_2.png', nombre:'CONGELADOR SOLAR 210L', Descripcion:'Panel solar 195Wp – 24VDC -- 2 unid Cable LAPPTHERM Solar XLS 4MM -- 20 unid Terminal LAPP hembra – 1 unid Terminal LAPP macho – 1 unid Bateria AGM sellada 12V/155A – 2 unid- Controlador MPPT 20/10A, 250W / 12V – 500W / 24V -100VDC – 1unid Nevera solar 100L – 12/24V – 1unid Características:Cuenta también con un sistema que reduce la escarcha y la humedad, por lo que es de fácil mantenimiento. También es un refrigerador ecológico ya que no contiene CFCs, usa refrigerante R-134a, que no daña la capa de ozono, de gran estabilidad química y térmica y una baja toxicidad, además de no ser inflamable.'},
              {src: '../../img/productos/inversor_2.png', nombre:'CONGELADOR SOLAR 235L', Descripcion:'Panel solar 195Wp – 24VDC -- 2 unid Cable LAPPTHERM Solar XLS 4MM -- 20 unid Terminal LAPP hembra – 1 unid Terminal LAPP macho – 1 unid Bateria AGM sellada 12V/155A – 1 unid- Controlador MPPT 20/10A, 250W / 12V – 500W / 24V -100VDC Nevera / Refrigerador 235L (8.1cu.ft) 12 / 24 – 1unid Características:Cuenta también con un sistema que reduce la escarcha y la humedad, por lo que es de fácil mantenimiento. También es un refrigerador ecológico ya que no contiene CFCs, usa refrigerante R-134a, que no daña la capa de ozono, de gran estabilidad química y térmica y una baja toxicidad, además de no ser inflamable.'},
              {src: '../../img/productos/inversor_2.png', nombre:'CONGELADOR SOLAR 310L', Descripcion:'Panel solar 195Wp – 24VDC -- 2 unid Cable LAPPTHERM Solar XLS 4MM -- 20 unid Terminal LAPP hembra – 1 unid Terminal LAPP macho – 1 unid Bateria AGM sellada 12V/155A – 2 unid- Controlador MPPT 20/10A, 250W / 12V – 500W / 24V -100VDC – 1unid Nevera solar 100L – 12/24V – 1unid Características: Cuenta también con un sistema que reduce la escarcha y la humedad, por lo que es de fácil mantenimiento. También es un refrigerador ecológico ya que no contiene CFCs, usa refrigerante R-134a, que no daña la capa de ozono, de gran estabilidad química y térmica y una baja toxicidad, además de no ser inflamable.'},
              {src: '../../img/productos/inversor_2.png', nombre:'CONGELADOR SOLAR 430L', Descripcion:'Panel solar 95Wp – 12VDC (mono) -- 1 unid Cable LAPPTHERM Solar XLS 4MM -- 20 unid Terminal LAPP hembra – 1 unid Terminal LAPP macho – 1 unid Bateria AGM sellada 12V/75A – 1 unid Controlador 12V – 10/10A – 1 unid Nevera/Refregerador 310 L (8.1cu.ft) 12/24V – 1unid Características: Cuenta también con un sistema que reduce la escarcha y la humedad, por lo que es de fácil mantenimiento. También es un refrigerador ecológico ya que no contiene CFCs, usa refrigerante R-134a, que no daña la capa de ozono, de gran estabilidad química y térmica y una baja toxicidad, además de no ser inflamable.'},
              {src: '../../img/productos/inversor_2.png', nombre:'CONGELADOR SOLAR 520L', Descripcion:'Panel solar – 2 unids Cable LAPPTHERM solar XLS 4MM – 20m Terminal LAPP hembra – 1 unid Terminal LAPP macho – 1 unid Bateria AGM sellada 12V/45A – 2 unid Controlador – 1 unid Nevera / Refrigerador 310L ( 1.8 cu.ft) 12 /24V Características: Una de las principales características del refrigerador solar, es el gabinete súper aislado, con una capa de 11 centímetros de aislamiento con una cubierta de acero galvanizado en el exterior y aluminio en la parte interior. Cuenta también con un sistema que reduce la escarcha y la humedad, por lo que es de fácil mantenimiento. También es un refrigerador ecológico ya que no contiene CFCs, usa refrigerante R-134a, que no daña la capa de ozono, de gran estabilidad química y térmica y una baja toxicidad, además de no ser inflamable.'},
      ]     
      }

  },
}
</script>