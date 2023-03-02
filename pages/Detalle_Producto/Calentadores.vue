<template>
    <div>
      <theheader/>
      <MobileNavigation/>
      <Calentadores/>
      <TheFooter style="background-color: #383737;"/>
    </div>
  </template>
  
  <script>
  import Theheader from '~/components/Theheader.vue'
  import Calentadores from '~/components/Productos/Detalle_Producto/Calentadores.vue';
  import TheFooter from '~/components/TheFooter.vue';
  import MobileNavigation from '~/components/MobileNavigation.vue';
  export default {
    components: { Theheader, TheFooter, MobileNavigation, Calentadores },
    
  }
  </script>
  