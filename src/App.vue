<template>
  <div id="app">
    <Menu msg="Welcome Bozha" />
  </div>
</template>

<script>
import Menu from "./components/Menu.vue";

export default {
  name: "App",
  components: {
    Menu,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background: #1e5e9a;
  padding: 0;
  margin: 0;
}
body {
  padding: 0;
  margin: 0;
  height: 100vh;
}
</style>
