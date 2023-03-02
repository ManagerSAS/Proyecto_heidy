<template>
    <div>
      <theheader/>
      <MobileNavigation/>
      <inversores/>
      <TheFooter style="background-color: #383737;"/>
    </div>
  </template>
  
  <script>
  import Theheader from '~/components/Theheader.vue'

  import TheFooter from '~/components/TheFooter.vue';
  import MobileNavigation from '~/components/MobileNavigation.vue';
import inversores from '~/components/Productos/Detalle_Producto/inversores.vue';
  
  export default {
    components: { Theheader, TheFooter, MobileNavigation, inversores },
    
  }
  </script>
  