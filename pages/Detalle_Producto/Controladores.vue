<template>
    <div>
      <theheader/>
      <MobileNavigation/>
      <Controladores/>
      <TheFooter style="background-color: #383737;"/>
    </div>
  </template>
  
  <script>
  import Theheader from '~/components/Theheader.vue'

  import TheFooter from '~/components/TheFooter.vue';
  import MobileNavigation from '~/components/MobileNavigation.vue';
import Controladores from '~/components/Productos/Detalle_Producto/Controladores.vue';
  
  export default {
    components: { Theheader, TheFooter, MobileNavigation, Controladores },
    
  }
  </script>
  