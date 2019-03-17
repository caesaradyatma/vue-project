<template>
  <section class="herobanner">
    <div class="row banner-img">
      <div class="col-sm-6 content">
          <!-- <img :src="src" :alt="caption" class="banner-img"> -->
          <h3><strong>Title</strong></h3>
          <p>short description</p>
          <a href="#" class="btn btn-primary">Get Started</a>
          <a href="#" class="btn btn-primary">Learn More</a>
      </div>
      <div class="col-sm-6 content">

      </div>
    </div>
  </section>
</template>

<script>
export default {
  name:'herobanner',
  data (){
    return {
      src:'https://st.motortrend.com/uploads/sites/10/2015/09/2015-BMW-M4-convertible-top-up-in-motion-winding-road.jpg',
      caption:'ini gambar',
    }
  }
}
</script>

<style scoped>
  .banner-img{
    height:100vh;
    width:100%;
    background:url('https://st.motortrend.com/uploads/sites/10/2015/09/2015-BMW-M4-convertible-top-up-in-motion-winding-road.jpg');
    background-position: center;
    background-size: cover;
    color:white;
    text-align: left;
  }

  .content {
    padding: 10%;
  }
</style>


