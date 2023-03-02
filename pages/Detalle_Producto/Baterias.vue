<template>
    <div>
      <theheader/>
      <MobileNavigation/>
      <baterias/>
      <TheFooter style="background-color: #383737;"/>
    </div>
  </template>
  
  <script>
  import Theheader from '~/components/Theheader.vue'
  import baterias from '~/components/Productos/Detalle_Producto/Baterias';
  import TheFooter from '~/components/TheFooter.vue';
  import MobileNavigation from '~/components/MobileNavigation.vue';
  
  export default {
    components: { Theheader, baterias,TheFooter, MobileNavigation },
    
  }
  </script>
  