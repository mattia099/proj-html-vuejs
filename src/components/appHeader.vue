<template>
  <header class="d-flex flex-column">
    <smallBannerContacts class="d-lg-block" />
    <div class="hero-section flex-grow-1">
      <nav class="navbar navbar-expand-lg navbar-dark bg-transparent">
        <div class="container text-uppercase">
          <a class="navbar-brand fw-bold" href="#"><span class="logo">N e x</span> G e n</a>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
            <ul class="navbar-nav gap-3">
              <li class="nav-item" v-for="( element,index ) in link" :key="index">
                <a class="nav-link"  href="#">{{ element }}</a>
              </li>
              <li class="nav-item">
                <button class="btn main-color">Get in Touch</button>
              </li>
            </ul>
          </div>
        </div>
      </nav>

      <div class="hero-section_content">
        <h1 class="big-title">Lead ~ <span class="logo second">Customer</span></h1>
        <p>Succesful strategies require data analysis, creativity and costumer focus, taking advantage of the latest technologies to offer excellent services</p>
        <button class="btn main-color mx-2">Get in Touch</button>
        <button class="btn second-color mx-2">Read More</button>
      </div>

    </div>
  </header>
</template>

<script>
import smallBannerContacts from './smallBannerContacts.vue';
  
export default{
  name : 'appHeader',  
  
  components: { 
    smallBannerContacts,
  },
  
  data : function(){
    return{
      link : [ 'Home', 'About', 'Services', 'Pricing', 'Blog']
    }
  }
}  

</script>


<style scoped lang="scss">
  header{
    height: 100vh;
    color: white;
    .hero-section{
      height: 100%;
      background-image: url('../assets/images/hero-image.png');
      background-position: bottom center;
      background-size: cover;
      position: relative;
      .navbar-dark .navbar-nav .nav-link{
        color: white !important;
        font-weight: 700;
      }
      
      .hero-section_content{
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate( -50%, -50% );
        max-width: 600px;
        text-align: center;
        
      }
      &::before{
        content: '';
        display: block;
        position: absolute;
        top: 0;
        bottom: 0;
        right: 0;
        left: 0;
        background-color: rgba($color: #000000, $alpha: 0.7);
      }

      
    }
  }
    
</style>
