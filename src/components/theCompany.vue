<template>
  <section>
    <div class="row align-items-center">

      <div class="col-12 col-md-6">
        <div class="row">
          <div class="col-lg-8 offset-lg-4">
            <div class="description">
              <h5 class="xsmall-title text-uppercase">About the network</h5>
              <h2 class="medium-title"><span class="logo second">The</span>Company</h2>
              <p>For 12 years we have been providing audit and warranty, financial advice, risk advice, taxes and related to select client</p>

              <div class="row py-5">
                <div class="col-6">
                  <i class="fas fa-award"></i>
                  <h5 class="icon-title">Tradition</h5>
                  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                </div>
                <div class="col-6">
                  <i class="fas fa-lock"></i>
                  <h5 class="icon-title">Security</h5>
                  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                </div>
                <div class="col-6">
                  <i class="far fa-edit"></i>
                  <h5 class="icon-title">Certificate</h5>
                  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                </div>
                <div class="col-6">
                  <i class="fas fa-graduation-cap"></i>
                  <h5 class="icon-title">Expertise</h5>
                  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="col-12 col-md-6">
        <figure class="back">
        </figure>
      </div>

    </div>

  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
  @import "../assets/scss/mixins.scss";
  section{
    color: $shark;
    .row{
    --bs-gutter-x: 0;
    }
  }
  
  .back{
    background-image: url('../assets/images/about-3.jpg');
    background-size: cover;
    min-width: 300px;
    aspect-ratio: 1/1;
  }
  .description{
      padding: 20px 10px;
      .logo.second{
      color: $blueLagoon;
      margin-right: 4px;
    }

    .icon-title{
      display: inline-block;
      font-weight: 700;
      color: $shark;
    }
    i{
      font-size: 25px;
      color: $blueLagoon;
      padding-right: 8px;
    }
  }
</style>