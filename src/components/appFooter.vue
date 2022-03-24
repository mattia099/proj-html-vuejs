<template>
  <footer>
    <div class="container py-5">
      <div class="row py-5">
        <div class="col-3">
          <div class="row gy-4">
            <div class="col-12">
              <h4 class="fw-bold text-uppercase mb-3"><span class="logo">N e x</span> G e n</h4>
            </div>
            <div class="col-12">
              <p class="sub-text">A functional HTML template for Corporate e Business.</p>
            </div>
            <div class="col-12 d-flex align-items-center gap-2">
              <i class="fas fa-phone"></i>
              <p class="sub-text">+1 (305) 1234-5678</p>
            </div> 
            <div class="col-12 d-flex align-items-center gap-2">
              <i class="fas fa-envelope"></i>
              <p class="sub-text">hello@example.com</p>
            </div>
            <div class="col-12 d-flex align-items-center gap-2">
              <i class="fas fa-map-marker-alt"></i>
              <p class="sub-text">Main Avenue, 987</p>
            </div>
            <div class="col-12">
              <button class="btn second-color">Get in touch</button>
            </div>
          </div>
        </div>
        <div class="col-3">
          <div class="card-item p-4">
            <h3>About</h3>
            <ul class="sub-text py-3">
              <li><i class="fa-solid fa-angle-right"></i><span>The Company</span></li>
              <li><i class="fa-solid fa-angle-right"></i><span>The Company</span></li>
              <li><i class="fa-solid fa-angle-right"></i><span>The Company</span></li>
              <li><i class="fa-solid fa-angle-right"></i><span>The Company</span></li>
              <li><i class="fa-solid fa-angle-right"></i><span>The Company</span></li>
              <li><i class="fa-solid fa-angle-right"></i><span>The Company</span></li>
            </ul>
          </div>
        </div>
        <div class="col-3">
          <div class="card-item p-4">
            <h3>Services</h3>
            <ul class="sub-text py-3">
              <li><i class="fa-solid fa-angle-right"></i><span>The Company</span></li>
              <li><i class="fa-solid fa-angle-right"></i><span>The Company</span></li>
              <li><i class="fa-solid fa-angle-right"></i><span>The Company</span></li>
              <li><i class="fa-solid fa-angle-right"></i><span>The Company</span></li>
              <li><i class="fa-solid fa-angle-right"></i><span>The Company</span></li>
              <li><i class="fa-solid fa-angle-right"></i><span>The Company</span></li>
            </ul>
          </div>
        </div>
        <div class="col-3">
          <div class="card-item p-4">
            <h3>Support</h3>
            <ul class="sub-text py-3">
              <li><i class="fa-solid fa-angle-right"></i><span>The Company</span></li>
              <li><i class="fa-solid fa-angle-right"></i><span>The Company</span></li>
              <li><i class="fa-solid fa-angle-right"></i><span>The Company</span></li>
              <li><i class="fa-solid fa-angle-right"></i><span>The Company</span></li>
              <li><i class="fa-solid fa-angle-right"></i><span>The Company</span></li>
              <li><i class="fa-solid fa-angle-right"></i><span>The Company</span></li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="post-footer">
      <div class="container">
        <div class="row py-4">
          <div class="col-6">
            <p class="sub-text">Enjoy the low price. We are tracking any intention of privacy</p>
          </div>
          <div class="col-6">
            <p class="text-end sub-text">@2020 NEXGEN is Prodly Powered by <span>Codings</span></p>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import '../assets/scss/mixins.scss';
  footer{
    color: white;
    background-color: $woodSmoke;
    
    p{
      margin-bottom:0;
    }
    .card-item{
      background-color: #19191F;
      border-radius: 10px; 
      ul{
        li{
          padding-bottom: 10px;
          i{
            font-size: 18px;
            padding-right: 10px;
          }
        }
      }
    }
    .post-footer{
      background-color: #0D0D11;
    }
  }
</style>