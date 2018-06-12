<template>
  <div id="app">
    <img src="./assets/logo.png">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <h2>Ура {{cl}}</h2>
    <ul>
      <li :key="item" v-for="item in list">
        <div>
          {{item}}
        </div>
      </li>
    </ul>
    
  </div>
</template>

<script>
export default {
  name: "app",
  data() {
    return {
      msg: "Welcome to Your Vue.js App",
      list: [1, 2, 3, 4, 5, 6],
      cl: "test"
    };
  }
};
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1,
h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  margin: 10px 0;
  span {
    display: inline-block;
  }
}

a {
  color: #42b983;
}
</style>
