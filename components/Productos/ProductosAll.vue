<template>
    <v-container fluid>
        <v-row align="center" justify="center">
            <v-col cols="12" sm="12" md="10" lg="8" align="center" justify="center">
                <v-row align="center" justify="center">
                    <v-col cols="12" sm="12" md="3" v-for="(inf, index) in productos" :key="index">
                        <div>
                            <img :src="inf.src" width="60%"/>
                            <p>{{ inf.nombre }}</p>
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
    export default {
        data() {
            return{
                //Aca se crea un arreglo con los productos
                productos:[
                    {src: '../../img/productos/bateria_2.png', nombre:'baterías', to:'/Detalle_Producto/Baterias'},
                    {src: '../../img/productos/Calentador-Ele.png', nombre:'calentadores electrico', to:'/Detalle_Producto/Calentadores'},
                    {src: '../../img/productos/controlador_de_carga.png', nombre:'Controladores de carga', to:'/Detalle_Producto/Controladores'},
                    {src: '../../img/productos/inversor_2.png', nombre:'Inversores', to:'/Detalle_Producto/inversores'},
                    {src: '../../img/productos/BombaSolarAutomatico.png', nombre:'Bombas Solares', to:'/Detalle_Producto/Bombas '},
                    {src: '../../img/productos/PAC-ACDC12-removebg-preview.png', nombre:'Aire acondicionado', to:'/Detalle_Producto/Aireacondicionado'},
                    {src: '../../img/productos/purificador_de_agua.png', nombre:'Purificadores de agua', to:'/Detalle_Producto/Purificadores'},
                    {src: '../../img/productos/refi_2.png', nombre:'Refrigeradores', to:'/Detalle_Producto/Refrigeradores'},
                ]
            }
            
        },
    }
</script>