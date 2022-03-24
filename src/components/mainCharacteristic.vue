<template>
  <section>
    <div class="container">
      <div class="row py-5 gy-3" >
        
        <div class="col-12 col-md-6 col-lg-4" v-for="(element,index) in cards" :key="index">
          <div class="card">
            <div class="icon-container align-self-start">
              <i :class="element.icon"></i>
            </div>
            <h4>{{element.title}}</h4>
            <p>{{element.description}}</p>
          </div>
        </div>
        
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name : 'mainCharacteristic',
  data : function(){
    return {
      cards :[
        {
          title : 'Human Capital',
          description : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Veritatis hic suscipit amet. Quasi, ipsum. Lorem, ipsum dolor.',
          icon : 'fas fa-user-friends'
        },
        {
          title : 'Core Business',
          description : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Veritatis hic suscipit amet. Quasi, ipsum. Lorem, ipsum dolor.',
          icon : 'fas fa-chart-pie'
        },
        {
          title : 'Performance',
          description : 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Veritatis hic suscipit amet. Quasi, ipsum. Lorem, ipsum dolor.',
          icon : 'fas fa-tachometer-alt'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
  @import '../assets/scss/mixins.scss';
  section{
    background-color: #e3e7df;
    color: $canvas;
    height: auto;
    .card{
      padding: 40px 30px;
      border-radius: 10px;
      &:hover{
        transform: translateY(-10px);
      }
      h4{
        padding-bottom: 16px;
      }
      .icon-container{
        border-radius: 50%;
        background-color: rgba($color: #39c4c6, $alpha: 0.2);
        padding: 5px 10px;
        color: #038483;
        margin-bottom: 15px;
        font-size: 18px;
      }
    }
  }
</style>