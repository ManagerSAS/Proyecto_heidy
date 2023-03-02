<template>
    <div>
      <theheader/>
      <MobileNavigation/>
      <purificadores/>
      <TheFooter style="background-color: #383737;"/>
    </div>
  </template>
  
  <script>
  import Theheader from '~/components/Theheader.vue'

  import TheFooter from '~/components/TheFooter.vue';
  import MobileNavigation from '~/components/MobileNavigation.vue';
import purificadores from '~/components/Productos/Detalle_Producto/purificadores.vue';
  
  export default {
    components: { Theheader, TheFooter, MobileNavigation, purificadores },
    
  }
  </script>
  