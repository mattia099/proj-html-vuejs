<template>
  <section>
    <div class="container py-5">
      <div class="row py-5">
        <div class="col-12 col-md-7">
          <div class="row align-items-center g-2">
            <div class="col-12"><h4 class="xsmall-title text-uppercase">Send a message</h4></div>
            <div class="col-12"><h2 class="medium-title">Get in <span class="logo second">Touch</span></h2></div>
            <p class="sub-text">We will respond to your message as soon as possible</p>
          </div>
          <div class="row gy-3 py-4">
            <div class="col-6">
              <input type="text" placeholder="Name">
            </div>
            <div class="col-6">
              <input type="text" placeholder="Email">
            </div>
            <div class="col-6">
              <input type="text" placeholder="Phone">
            </div>
            <div class="col-6">
              <input type="text" placeholder="More Info">
            </div>
            <div class="col-12">
              <input class="big" type="text" placeholder="Message">
            </div>
            <div class="col-12">
              <button class="btn main-color">Send</button>
            </div>
          </div>
        </div>

        <div class="col-12 col-md-5">
          <div class="row g-2">
            <div class="col-12">
              <h4>Example Inc.</h4>
            </div>
            <div class="col-12">
              <p class="sub-text">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
            </div>
            <div class="col-12">
              <p class="sub-text">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
            </div>
            <div class="col-12 d-flex align-items-center gap-2">
              <div class="icon-container">
                <i class="fas fa-phone"></i>
              </div>
              <p class="lagoon">+1 (305) 1234-5678</p>
            </div>
            <div class="col-12 d-flex align-items-center gap-2">
              <div class="icon-container">
                <i class="fas fa-envelope"></i>
              </div>
              <p class="lagoon">hello@example.com</p>
            </div>
            <div class="col-12 d-flex align-items-center gap-2">
              <div class="icon-container">
                <i class="fas fa-map-marker-alt"></i>
              </div>
              <p class="lagoon">Main Avenue, 987</p>
            </div>
            <div class="col-12">
              <button class="btn second-color lagoon">View map</button>
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
@import '../assets/scss/mixins.scss';
  section{
    color: $canvas;
    .logo.second{
      color: $blueLagoon;
    }
    input{
      width: 100%;
      padding: 10px 14px;
      background-color: #ECECEC;
      border: none;
    } 
    .big{
      padding-bottom:70px;
    }
    .icon-container{
        border-radius: 50%;
        background-color: rgba($color: #39c4c6, $alpha: 0.2);
        padding: 5px 10px;
        color: #038483;
        margin-bottom: 15px;
        font-size: 18px;
      } 
    .lagoon{
      color: $blueLagoon;
      font-size:17px;
    }
    h4{
      margin-bottom:16px;
    }
  }
</style>