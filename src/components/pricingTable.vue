<template>
  <section>
    <div class="container">
      <div class="row gy-2">
        <div class="col-12"><h4 class="xsmall-title text-center text-uppercase">Monthly plans</h4></div>
        <div class="col-12"><h2 class="medium-title text-center"><span class="logo second">Pricing</span> Table</h2></div>
        <div class="col-md-6 offset-md-3"><p class="sub-text text-center">We can help you deliver and execute your future, wherever you compete, using the latest technologies, from strategy development to implementation.</p></div>
        
        <div class="col-12 col-md-6 col-lg-4">
          <div class="card-item d-flex flex-column align-items-center gap-2">
            <i class="fas fa-arrow-right"></i>
            <i class="fas fa-rocket"></i>
            <h4 class="card_title">Standard</h4>
            <p class="card_small-text">$<span class="card_price">490</span>/mo</p>
            <ul class="align-self-start">
              <li class="d-flex justify-content-between align-items-center"><span class="sub-text">Standard Accounting</span><i class="fas fa-check"></i></li>
              <li class="d-flex justify-content-between align-items-center"><span class="sub-text">Platform Access</span><i class="fas fa-check"></i></li>
              <li class="d-flex justify-content-between align-items-center"><span class="sub-text">Business Orientation</span><i class="fas fa-times"></i></li>
              <li class="d-flex justify-content-between align-items-center"><span class="sub-text">Dedicated Consultant</span><i class="fas fa-times"></i></li>
              <li class="d-flex justify-content-between align-items-center"><span class="sub-text">Personal Assistance</span><i class="fas fa-times"></i></li>
            </ul>
          </div>
        </div>
        
        <div class="col-12 col-md-6 col-lg-4">
          <div class="card-item d-flex flex-column align-items-center gap-2">
            <i class="fas fa-arrow-right"></i>
            <i class="fas fa-briefcase"></i>
            <h4 class="card_title">Professional</h4>
            <p class="card_small-text">$<span class="card_price">890</span>/mo</p>
            <ul class="align-self-start">
              <li class="d-flex justify-content-between align-items-center"><span class="sub-text">Standard Accounting</span><i class="fas fa-check"></i></li>
              <li class="d-flex justify-content-between align-items-center"><span class="sub-text">Platform Access</span><i class="fas fa-check"></i></li>
              <li class="d-flex justify-content-between align-items-center"><span class="sub-text">Business Orientation</span><i class="fas fa-check"></i></li>
              <li class="d-flex justify-content-between align-items-center"><span class="sub-text">Dedicated Consultant</span><i class="fas fa-times"></i></li>
              <li class="d-flex justify-content-between align-items-center"><span class="sub-text">Personal Assistance</span><i class="fas fa-times"></i></li>
            </ul>
            <div class="badge-popular">Most Popular</div>
          </div>
        </div>
         <div class="col-12 col-md-6 col-lg-4">
          <div class="card-item d-flex flex-column align-items-center gap-2">
            <i class="fas fa-arrow-right"></i>
            <i class="far fa-gem"></i>
            <h4 class="card_title">Ultimate</h4>
            <p class="card_small-text">$<span class="card_price">1.390</span>/mo</p>
            <ul class="align-self-start">
              <li class="d-flex justify-content-between align-items-center"><span class="sub-text">Standard Accounting</span><i class="fas fa-check"></i></li>
              <li class="d-flex justify-content-between align-items-center"><span class="sub-text">Platform Access</span><i class="fas fa-check"></i></li>
              <li class="d-flex justify-content-between align-items-center"><span class="sub-text">Business Orientation</span><i class="fas fa-check"></i></li>
              <li class="d-flex justify-content-between align-items-center"><span class="sub-text">Dedicated Consultant</span><i class="fas fa-check"></i></li>
              <li class="d-flex justify-content-between align-items-center"><span class="sub-text">Personal Assistance</span><i class="fas fa-check"></i></li>
            </ul>
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
      cards : [
        {
          title : '',
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
  @import '../assets/scss/mixins.scss';
  h4{
    margin-bottom:0;
  }
  
  section{
    background-color: $greyNurse;
    color: $canvas;
    padding: 80px 0;
    .logo.second{
      color: $blueLagoon;
    }
    .card-item{
      padding: 40px 30px;
      background-color: white;
      border-radius: 10px;
      position: relative;
      .badge-popular{
        position: absolute;
        top: 10px;
        left: 0;
        width: 55px;
        background-color: #00A6A6;
        color: white;
        border-top-right-radius: 30px;
        border-bottom-right-radius: 30px;
        font-size: 11px;
        padding: 5px;
        line-height: 12px;
      }
      i{
        font-size: 30px;
        color: $blueLagoon;
      }
      i:first-child{
        font-size: 25px;
        position: absolute;
        top: 30px;
        right: 30px;
        display: none
      }

      &:hover i:first-child{
        display: block;
      }
      .card_title{
        font-weight: 700;
        font-size: 1.8rem;
      }
      .card_small-text{
        font-weight: 400;
        font-size: 18px;
        color: $blueLagoon;
        .card_price{
          font-size: 2.0rem;
          font-weight: 700;
        }
      }
      ul{
        width: 100%;
        li{
          padding-bottom: 12px;
          i{
            font-size: 18px;
          }
        }
      }
      
    }
  }
</style>