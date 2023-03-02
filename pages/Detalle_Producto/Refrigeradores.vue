<<template>
    <div>
      <theheader/>
      <MobileNavigation/>
      <Refrigeradores/>
      <TheFooter style="background-color: #383737;"/>
    </div>
  </template>
  
  <script>
  import Theheader from '~/components/Theheader.vue'

  import TheFooter from '~/components/TheFooter.vue';
  import MobileNavigation from '~/components/MobileNavigation.vue';
import Refrigeradores from '~/components/Productos/Detalle_Producto/Refrigeradores';
  export default {
    components: { Theheader, TheFooter, MobileNavigation, Refrigeradores },
    
  }
  </script>
  