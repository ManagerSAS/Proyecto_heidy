<template>
    <div>
      <theheader/>
      <MobileNavigation/>
      <welcome texto="PRODUCTOS"/>
      <ProductosAll/>
      <TheFooter style="background-color: #383737;"/>
    </div>
  </template>
  
  <script>
  import Theheader from '~/components/Theheader.vue'
  import welcome from '~/components/Productos/welcome.vue';
  import ProductosAll from '~/components/Productos/ProductosAll.vue';
  import TheFooter from '~/components/TheFooter.vue';
  import MobileNavigation from '~/components/MobileNavigation.vue';
  
  export default {
    components: { Theheader, welcome,ProductosAll, TheFooter, MobileNavigation },
    
  }
  </script>
  