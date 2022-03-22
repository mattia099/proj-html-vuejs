<template>
  <section>
    <div class="container">
      <div class="row py-5">
        <div class="col">
          <div class="card">
            <div class="icon-container align-self-start">
              <i class="fas fa-user-friends"></i>
            </div>
            <h4>Human Capital</h4>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Veritatis hic suscipit amet. Quasi, ipsum. Lorem, ipsum dolor.</p>
          </div>
        </div>
        <div class="col">
          <div class="card">
            <div class="icon-container align-self-start">
              <i class="fas fa-chart-pie"></i>
            </div>
            <h4>Core Business</h4>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Aspernatur inventore minus nam nemo laboriosam commodi?</p>
          </div>
          </div>
        <div class="col">
          <div class="card">
            <div class="icon-container align-self-start">
              <i class="fas fa-tachometer-alt"></i>
            </div>
            <h4>Performance</h4>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corporis quam ipsam id consequatur reiciendis nostrum!</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>

export default {
  name : 'mainCharacteristic',
}
</script>

<style lang="scss" scoped>
  section{
    background-color: #e3e7df;
    color: #1e2223;
    height: auto;
    .card{
      padding: 40px 30px;
      border-radius: 10px;
      &:hover{
        transform: translateY(-10px);
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