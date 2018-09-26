<template>
  <div id="app">
    <img alt="URSAL" src="./assets/ursal.png">
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <side-bar> </side-bar>
  </div>
</template>

<script>
import SideBar from './components/SideBar/SideBar.vue'

export default {
  name: 'app',
  components: {
    'side-bar' : SideBar
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
