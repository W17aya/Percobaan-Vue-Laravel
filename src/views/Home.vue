<template>
    <div class="home">
        <HeaderShayna/> 
        <HeroShayna/>
        <WomenShayna/>
        <GaleriShayna/>
    </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import HeaderShayna from '@/components/HeaderShayna.vue';
import HeroShayna from '@/components/HeroShayna.vue';
import WomenShayna from '@/components/WomenShayna.vue';
import GaleriShayna from '@/components/GaleriShayna.vue';

export default {
  name: 'Home',
  components: {
    HeaderShayna,
    HeroShayna,
    WomenShayna,
    GaleriShayna
  }
}
</script>
