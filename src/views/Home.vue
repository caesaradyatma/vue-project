<template>
  <div class="home">
    <Featured />
    <hr>
    <HeroBanner />
    <hr>
    <Featured :vertical=true />
  </div>
</template>

<script>
// @ is an alias to /src
import Featured from '@/components/Sections/Featured.vue';
import HeroBanner from '@/components/Banners/HeroBanner.vue';

export default {
  name: 'home',
  components: {
    HeroBanner,
    Featured,
  },
};
</script>
