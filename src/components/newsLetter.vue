<template>
  <section>
    <div class="container py-5">
      <div class="row py-5">
        <div class="col-12 col-md-6">
          <div class="row gap-4">
            <div class="col-12"><h4 class="xsmall-title text-uppercase">NewsLetter</h4></div>
            <div class="col-12"><h2 class="medium-title"><span class="logo second">Know</span> First</h2></div>
            <div class="col-12"><p class="sub-text">Follow closely and receive content about our compony and the news of the current market.</p></div>
          </div>
        </div>
        <div class="col-12 col-md-6">
          <div class="row gap-4">
            <div class="col-12">
              <input class="main-input" type="text" placeholder="Name">
            </div>
            <div class="col-12">
              <input class="main-input" type="text" placeholder="email">
            </div>  
            <div class="col-12">
              <button class="btn main-color">Subscribe</button>
            </div>
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
  section{
    background-image: url('../assets/images/bg-1.jpg');
    background-position: center;
    background-size: cover;
    color: white;
    .container{
      max-width: 970px;
      .main-input{
        width: 100%;
        padding: 10px 8px;
        border-radius: 4px;
        background-color: rgba($color: white, $alpha: 0.5);
        border: none;
      }
    }
  }
</style>