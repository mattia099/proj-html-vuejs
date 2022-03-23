<template>
  <section class="py-5">
    <div class="container py-5">
      <div class="row align-items-center g-2">
        <div class="col-12"><h4 class="xsmall-title text-uppercase">Our business areas</h4></div>
        <div class="col-12"><h2 class="medium-title">Latest <span class="logo second">News</span></h2></div>
        <div class="col-9"><p>Every week we publish content about what is best in the business world</p></div>
        <div class="col-3 text-end"><button class="btn main-color">See all</button></div>
      </div> 

      <div class="row gy-4 py-5">
        <div class="col-12 col-md-6 col-lg-4">
          <div class="card-item">
            <img src="../assets/images/news-1.jpg" alt="">
            <h4 class="">Increasing creativity is possible for everyone</h4>
          </div>
        </div>

        <div class="col-12 col-md-6 col-lg-4">
          <div class="card-item">
            <img src="../assets/images/news-2.jpg" alt="">
            <h4 class="">Becouse market research is part of the business plan</h4>
          </div>
        </div>

        <div class="col-12 col-md-6 col-lg-4">
          <div class="card-item">
            <img src="../assets/images/news-3.jpg" alt="">
            <h4 class="">Working from home is now a trend</h4>
          </div>
        </div>
      </div>

    </div> 
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import '../assets/scss/mixins.scss';
  section{
    color: $canvas;
    p{
      margin-bottom: 0;
    }
    .logo.second{
      color: $blueLagoon;
    }
    .card-item{
      max-width: 100%;
      border-radius: 10px;
      overflow: hidden;
      position: relative;
      &::before{
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        bottom: 0;
        right: 0;
        background-color: rgba($color: #000000, $alpha: 0.6);
      }    
      h4{
        position: absolute;
        bottom: 45px;
        left: 0px;
        color: white;
        font-weight: 700;
        font-size: 1.8rem;
        text-align: center;
        padding: 10px;
      }
    }
  }
</style>