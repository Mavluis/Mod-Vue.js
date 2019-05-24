<template>
  <div id="app">
    <img alt="Vue logo" src="./components/honda.jpg">
    <Coche msg="HONDA"/>
  </div>
</template>

<script>
import Coche from './components/Coche.vue'

export default {
  name: 'app',
  components: {
    Coche
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
