<template>
  <div id="app">
<MainPage></MainPage>
<Footer/>
  </div>
</template>

<script>
import MainPage from './components/MainPage.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    MainPage,
    Footer
  }
}
</script>

<style lang="scss">
@import './assets/style/index.scss';



</style>
