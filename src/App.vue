<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <Menu msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Menu from './components/Menu.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld
    Menu
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
  margin-top: 20px;
}
body {
  /* background: #89CFD1; */
  background: rgb(139,209,209);
  background: linear-gradient(180deg, rgba(137,207,209,1) 39%, rgba(87,182,173,1) 100%);
  height: 100vh;
}
</style>
