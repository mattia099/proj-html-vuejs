<template>
  <div id="app">
    <appHeader />
  </div>
</template>

<script>
import appHeader from './components/appHeader.vue'

export default {
  name: 'App',
  components: {
    appHeader,
  }
}
</script>

<style lang="scss">
@import "bootstrap/scss/bootstrap";
@import '~@fortawesome/fontawesome-free/css/all.css';
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
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
</style>
