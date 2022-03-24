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
        <div class="col-12 col-md-6 col-lg-4" v-for="(element,index) in cards" :key="index">
          <div class="card-item d-flex flex-column justify-content-end" 
          :style="{ 'background-image': 'url(' + element.image + ')' }" 
          @mouseover="element.upHere = true" @mouseleave="element.upHere = false">
            <div class="user d-flex justify-content-between" v-if="element.upHere == true">
              <div class="d-flex align-items-center gap-2"><i class="far fa-user"></i><span>{{element.user}}</span></div>
              <div class="d-flex align-items-center gap-2"><i class="far fa-clock"></i><span>{{element.time}}</span></div>
            </div>
            
            <div class="info-container">
            <h4 class="">{{element.title}}</h4>
            <p v-if="element.upHere == true">{{element.description}}</p>
            </div>
            
          </div>
        </div>

        
      </div>

    </div> 
  </section>
</template>

<script>
export default {
  data : function(){
    return{
      cards:[
        {
          image : require('../assets/images/news-1.jpg'),
          title : 'Increasing creativity is possible for everyone',
          description : 'lorem ipsud dolor sit amet, consectetur adipiscing elit.',
          user : 'Andrea Miller',
          time : '2 Days Ago',
          upHere : 'false'
        },
        {
          image : require('../assets/images/news-2.jpg'),
          title : 'Becouse market research is part of the business plan',
          description : 'lorem ipsud dolor sit amet, consectetur adipiscing elit.',
          user : 'Mattia Puglisi',
          time : '3 Days Ago',
          upHere : 'false'
        },
        {
          image : require('../assets/images/news-3.jpg'),
          title : 'Working from home is now a trend',
          description : 'lorem ipsud dolor sit amet, consectetur adipiscing elit.',
          user : 'Gina Rossi',
          time : '1 Hour Ago',
          upHere : 'false'
        }
      ]
    }
  }
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
      min-height: 400px;
      background-position: center;
      background-size: cover;
      &::before{
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        bottom: 0;
        right: 0;
        background-color: rgba($color: #000000, $alpha: 0.7);
      } 
      .info-container{
        z-index: 2;
        padding: 50px 0px;
        h4{
        color: white;
        font-weight: 700;
        font-size: 1.8rem;
        text-align: center;
        padding-bottom: 20px;
        padding-right: 50px;
        padding-left: 50px;
        z-index:2;
        }
        p{
        color: white;
        text-align: center;
        padding: 0 50px;
        z-index: 2;
        font-size: 1.1rem;
        }
      }
      .user{
        position: absolute;
        top: 0;
        left: 0;
        z-index: 1;
        color: white;
        width: 100%;
        padding: 50px;
        font-size: 1.1rem;
      }
    }
  }
</style>