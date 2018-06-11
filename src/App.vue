<template>
  <div id="app">
    <div ref="logo">

    </div>
    <div class="lenossa">
      teste
    </div>
  </div>
</template>

<script>
import '@/assets/styles.css'
import lottie from 'lottie-web'

export default {
  name: 'App',
  mounted () {
    let animation = lottie.loadAnimation({
      container: this.$refs.logo,
      renderer: 'svg',
      // loop: true,
      autoplay: true,
      path: 'https://www.jasonbase.com/things/4K63.json'
    })
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
