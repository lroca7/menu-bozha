<template>
  <div class="hello">
    <div class="languages">
      <img src="../assets/usa.png" @click="selectLanguage('english')" />
      <img src="../assets/colombia.png" @click="selectLanguage('spanish')" />
    </div>

    <img v-if="language === 'spanish'" src="../assets/SP_0001.jpg" alt="Menu" />
    <img v-else src="../assets/EN_0001.jpg" alt="Menu" />

    <img v-if="language === 'spanish'" src="../assets/SP_0002.jpg" alt="Menu" />
    <img v-else src="../assets/EN_0002.jpg" alt="Menu" />

    <img
      v-if="language === 'spanish'"
      src="../assets/Brunch_0001.jpg"
      alt="Menu"
    />
    <img v-else src="../assets/Brunch_0002.jpg" alt="Menu" />

    <img
      v-if="language === 'spanish'"
      src="../assets/Licores_0001.jpg"
      alt="Menu"
    />
    <img v-else src="../assets/Licores_0002.jpg" alt="Menu" />
  </div>
</template>

<script>
export default {
  name: "Menu",
  props: {
    msg: String,
  },
  data() {
    return {
      language: "spanish",
    };
  },

  methods: {
    selectLanguage(languageSelected) {
      this.language = languageSelected;
    },
  },
};
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
body {
}
.hello {
  background: #fff;
  max-width: 1200px;
  margin: 0 auto;
}
.title {
  font-size: 42px;
  color: #446fc2;
  font-weight: bold;
}
.languages {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
}
.languages img {
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
