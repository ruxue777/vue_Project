<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HW msg="测试git！"/>
    <div>123</div>
  </div>
</template>

<script>
import HW from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HW 
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} 
</style>
