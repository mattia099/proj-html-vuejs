<template>
  <div id="app">
    <appHeader />
    <mainCharacteristic />
  </div>
</template>

<script>
import appHeader from './components/appHeader.vue';
import mainCharacteristic from './components/mainCharacteristic.vue';
export default {
  name: 'App',
  components: {
    appHeader,
    mainCharacteristic
  }
}
</script>

<style lang="scss">
@import "bootstrap/scss/bootstrap";
@import '~@fortawesome/fontawesome-free/css/all.css';
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  font-size: 15px;
}
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

ul{
  list-style-type: none;
  padding-left: 0;
  margin-bottom: 0;
}

.main-color{
  color:white;
  background-color: #038483;
  text-transform: uppercase;
  font-weight: 700;
  &:hover{
    background-color: #39c4c6;
    color: white;
  }
}

.second-color{
  color:white;
  background-color: transparent;
  text-transform: uppercase;
  font-weight: 700;
  border: 1px solid #038483;
  &:hover{
    background-color: #038483;
    color: white;
  }
}
</style>
