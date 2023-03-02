<template>
    <div>
      <theheader/>
      <MobileNavigation/>
      <aireacondicionado/>
      <TheFooter style="background-color: #383737;"/>
    </div>
  </template>
  
  <script>
  import Theheader from '~/components/Theheader.vue'
  import aireacondicionado from '~/components/Productos/Detalle_Producto/Aireacondicionado';
  import TheFooter from '~/components/TheFooter.vue';
  import MobileNavigation from '~/components/MobileNavigation.vue';
  
  export default {
    components: { Theheader, aireacondicionado,  TheFooter, MobileNavigation },
    
  }
  </script>
  