<template>
  <section>
    <div class="container">
      <div class="row g-4">
        <div class="col-12"><h4 class="xsmall-title text-uppercase">Our Business Areas</h4></div>
        <div class="col-12"><h2 class="medium-title">Excellence in <span class="logo second">Services</span></h2></div>
        <div class="col-9"><p>We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of experienced and renowned professionals. These are some options that you can hire</p></div>
        <div class="col-3 text-end"><button class="btn second-color">See all</button></div>
      </div>  
    
      <div class="row g-4">
        <div class="col-12 col-md-6 col-lg-4" v-for="(element,index) in cards" :key="index">
          <div class="card-item d-flex flex-column g-5">
            <i :class="element.icon"></i>
            <h4>{{element.title}}</h4>
            <p class="sub-text">{{element.description}}</p>
            <button class="btn second-color align-self-start">Read More</button>
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
      cards :[
        {
          title : 'Audit e Assurance',
          description : 'Lorem, ipsum dolor sit amet consectetur adipisicing elit.',
          icon : 'fas fa-network-wired'
        },
        {
          title : 'Financial Advisory',
          description : 'Lorem, ipsum dolor sit amet consectetur adipisicing elit.',
          icon : 'fas fa-briefcase'
        },
        {
          title : 'Analytics and MeA',
          description : 'Lorem, ipsum dolor sit amet consectetur adipisicing elit.',
          icon : 'fas fa-chart-bar'
        },
        {
          title : 'Middle Marketing',
          description : 'Lorem, ipsum dolor sit amet consectetur adipisicing elit.',
          icon : 'fas fa-plane'
        },
        {
          title : 'Legal Consulting',
          description : 'Lorem, ipsum dolor sit amet consectetur adipisicing elit.',
          icon : 'fas fa-globe-americas'
        },
        {
          title : 'Regulatory Risk',
          description : 'Lorem, ipsum dolor sit amet consectetur adipisicing elit.',
          icon : 'far fa-folder'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/mixins.scss';
  section{
    color: white;
    background-color: $woodSmoke;
    padding: 80px 0;
    .card-item{
      padding: 20px;
      background-color: #19191F;
      i{
        font-size: 30px;
        color: $blueLagoon;
        margin-bottom: 0.8rem;
      }
    
    &:hover i{
      color: white;
    }
    &:hover .sub-text{
      opacity: 1.0;
    }
    }
  }
</style>