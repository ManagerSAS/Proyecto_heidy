<template>
  <div>
    <theheader/>
    <MobileNavigation/>
    <Welcome/>
    <Services/>
    <Cta style="background-image: url('/Cta.png');background-position: center;  background-size: cover; background-repeat: no-repeat;"/>
    <about/>
    <TheFooter style="background-color: #383737;"/>
  </div>
</template>

<script>
import Theheader from '~/components/Theheader.vue'
import Welcome from '~/components/index/Welcome.vue';
import Services from '~/components/index/Services.vue';
import Cta from '~/components/index/Cta.vue';
import about from '~/components/index/about.vue';
import TheFooter from '~/components/TheFooter.vue';
import MobileNavigation from '~/components/MobileNavigation.vue';

export default {
  components: { Theheader, Welcome, Services, Cta, about, TheFooter, MobileNavigation },
  
}
</script>
