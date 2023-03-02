<template>
    <div>
      <theheader/>
      <MobileNavigation/>
      <Bombas/>
      <TheFooter style="background-color: #383737;"/>
    </div>
  </template>
  
  <script>
  import Theheader from '~/components/Theheader.vue'
  import Bombas from '~/components/Productos/Detalle_Producto/Bombas.vue';
  import TheFooter from '~/components/TheFooter.vue';
  import MobileNavigation from '~/components/MobileNavigation.vue';
  
  export default {
    components: { Theheader, Bombas,  TheFooter, MobileNavigation },
    
  }
  </script>
  