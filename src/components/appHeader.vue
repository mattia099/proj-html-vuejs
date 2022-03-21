<template>
  <header>
    <smallBannerContacts />
    <div class="hero-section">
      <nav class="navbar navbar-expand-lg navbar-dark bg-transparent">
        <div class="container-xl text-uppercase">
          <a class="navbar-brand" href="#">NexGen</a>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
            <ul class="navbar-nav">
              <li class="nav-item">
                <a class="nav-link active" aria-current="page" href="#">Home</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">About</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">Services</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">Pricing</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">Blog</a>
              </li>
            </ul>
          </div>
        </div>
      </nav>
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
}  

</script>


<style scoped lang="scss">
  header{
    height: calc(100vh - 40px);
    
    .hero-section{
      height: 100%;
      background-image: url('../assets/images/hero-image.png');
      background-position: bottom center;
      background-size: cover;
      position: relative;
      &::before{
        content: '';
        display: block;
        position: absolute;
        top: 0;
        bottom: 0;
        right: 0;
        left: 0;
        background-color: rgba($color: #000000, $alpha: 0.3);
      }
    }
  }
    
</style>
