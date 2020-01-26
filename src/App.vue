<template>
  <div id="app">
    <div>
      <h1>{{msg}}</h1>
    </div>
    <formList></formList>
  </div>
</template>


<script>
import FormList from "./components/FormList";

export default {
  components: {
    FormList
  },
  name: "app",
  data() {
    return {
      msg: "Welcome to Your Vue.js App"
    };
  }
};
</script>

<style>
html {
  box-sizing: border-box;
}
*,
*:before,
*:after {
  box-sizing: inherit;
}

body {
  margin: 0;
  padding: 0;
  width: 100vw;
  height: 100vh;
  font-family: "Gill Sans Extrabold", Helvetica, sans-serif;
}

#app {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-flow: wrap;
  margin: 10px;
}
</style>
