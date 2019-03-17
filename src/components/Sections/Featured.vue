<template>
  <section class="featured">
    <div class="row" v-if="vertical">
      <div class="col-sm-12">
        <Card />
        <CardInvert />
      </div>
    </div>
    <div class="row" v-else>
      <div class="col-sm-4">
        <center>
          <Card :vertical=true :button=true />
        </center>
      </div>
      <div class="col-sm-4">
        <center>
          <Card />
          <Card />
          <Card />
        </center>
      </div>
      <div class="col-sm-4">
        <center>
          <Card :vertical=true :button=true />
          <a href="#">SEE ALL FEATURED ></a>
        </center>
      </div>
    </div>
  </section>
</template>

<script>
import Card from '@/components/Cards/Card.vue';
import CardInvert from '@/components/Cards/CardInvert.vue';

export default {
  name: 'featured',
  components: {
    Card,
    CardInvert,
  },
  props: {
    vertical: Boolean,
  }
}
</script>

