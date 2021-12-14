<template>
  <div id="app">
    <Header/>
    <Jumbotron/>
    <Main/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/macro/Header.vue';
import Main from './components/macro/Main.vue';
import Jumbotron from './components/macro/Jumbotron.vue';
import Footer from './components/macro/Footer.vue';


export default {
  name: 'App',
  components: {
    Header,
    Main,
    Jumbotron,
    Footer
  }
}
</script>

<style lang="scss">
@import './assets/style/global.scss';
</style>
