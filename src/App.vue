<template>
  <div id="app">
    <appHeader />
    <mainCharacteristic />
    <theCompany />
    <businessArea />
    <pricingTable />
    <latestNews />
    <newsLetter />
    <sendMessage />
    <appFooter />
  </div>
</template>

<script>
import appHeader from './components/appHeader.vue';
import mainCharacteristic from './components/mainCharacteristic.vue';
import theCompany from './components/theCompany.vue';
import businessArea from './components/businessArea.vue';
import pricingTable from './components/pricingTable.vue';
import latestNews from './components/latestNews.vue';
import newsLetter from './components/newsLetter.vue'
import sendMessage from './components/sendMessage.vue'
import appFooter from './components/appFooter.vue'
export default {
  name: 'App',
  components: {
    appHeader,
    mainCharacteristic,
    theCompany,
    businessArea,
    pricingTable,
    latestNews,
    newsLetter,
    sendMessage,
    appFooter
  }
}
</script>

<style lang="scss">
@import "bootstrap/scss/bootstrap";
@import '~@fortawesome/fontawesome-free/css/all.css';
@import "./assets/scss/mixins.scss";

#app {
  font-size: 15px;
  font-family: 'Arial Narrow Bold', sans-serif
}

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
img{
  max-width: 100%;
}
ul{
  list-style-type: none;
  padding-left: 0;
  margin-bottom: 0;
}
figure{
  margin: 0;
}
h4{
    margin-bottom: 0;
}

</style>
