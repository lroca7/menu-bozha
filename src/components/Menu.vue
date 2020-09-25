<template>
  <div class="hello">
    <div class='title'>Menu</div>
    <img src='../assets/1.png' />
  </div>
</template>

<script>
export default {
  name: 'Menu',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
img {
    width: 100%;
}
.title {
  font-family: 'Chewy', cursive;
  font-size: 24px;
  color: #665946;
}
</style>
