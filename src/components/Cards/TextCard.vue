<template>
  <div class="card">
    <div v-if="vertical">
      <center>
        <img class="card-img-top img-card" :src="img" alt="Card image cap">
      </center>
      <div class="card-body">
        <h5 v-modal="title">{{title}}</h5>
        <p v-modal="text">{{text}}</p>
        <a :href="link" class="btn btn-primary" v-if="button" :link="link">{{link}}</a>
      </div>
    </div>
    <div v-else>
      <div class="row">
        <div class="col-sm-5">
          <h3>{{order}}</h3>
        </div>
        <div class="col-sm-7">
          <div class="card-body">
            <h5 v-modal="title">{{title}}</h5>
            <p v-modal="text">{{text}}</p>
            <a :href="link" class="btn btn-primary" v-if="button" :link="link">{{link}}</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name:'card',
  data() {
    return {
      title: 'Default title',
      text: 'default text',
      button: true,
      link: 'www.google.com',
      img: 'https://st.motortrend.com/uploads/sites/5/2017/02/2016-BMW-M2-Coupe-front-three-quarter-burnout1.jpg',
    }
  },
  props: {
    vertical: Boolean,
    button: Boolean,
    urlParam: String,
    order: String,
  }
}
</script>

<style scoped>
  .img-card{
    height:100%;
    width:100%;
  }

  .card{
    text-align:left;
    padding: 2%;

    margin-bottom: 2%;
  }
</style>


