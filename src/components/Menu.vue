<template>
  <div class="hello">
    <div class='languages'>
      <img src='../assets/usa.png' @click="selectLanguage('english')" />
      <img src='../assets/colombia.png'  @click="selectLanguage('spanish')"/>
    </div>
    <div class="options__menu">
      <div v-if="language === 'spanish'" class='title'>Menú</div>    
      <div v-else class='title'>Menu</div>
    </div>
    
    
    
    <img v-if="language === 'spanish'" src='../assets/1.jpg' alt="Menu" />
    <img v-else src='../assets/2.jpg' alt="Menu" />

    <img v-if="language === 'spanish'" src='../assets/bozhayuno.jpg' alt="Menu" />
    <img v-else src='../assets/bozhayuno_eng.jpg' alt="Menu" />
  </div>
</template>

<script>
export default {
  name: 'Menu',
  props: {
    msg: String
  },
  data() {
        return {
            language: 'spanish',
        }
    },

  methods: {
    selectLanguage(languageSelected) {
      this.language = languageSelected
    }
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
  /* font-family: 'Chewy', cursive; */
  font-size: 42px;
  /* color: #665946; */
  color: #446FC2;
  font-weight: bold;
}
.languages {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
}
.languages img{
  width: 30px;
  padding: 0px 5px;
}

.options__menu {
  display: flex;
  justify-content: center;
  margin-left: 10%;
  .option2 {
    margin-left: 70px;
  }

}

@media screen and (max-width: 1200px) {
.title {
  font-size: 1rem;
}
}
</style>
