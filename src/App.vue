<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <Amedida msg="" />
  </div>
</template>

<script>
import Amedida from "./components/Amedida.vue";

export default {
  name: "App",
  components: {
    Amedida,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
