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
  margin-top: 20px;
}
body {
  /* background: rgb(139, 209, 209);
  background: linear-gradient(
    180deg,
    rgba(137, 207, 209, 1) 39%,
    rgba(87, 182, 173, 1) 100%
  ); */
  height: 100vh;
}
</style>
