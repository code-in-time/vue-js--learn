<template>
  <div class="app">
    <Main2 />
    <Bottom/>
  </div>
</template>

<script>
import Main2 from "./components/Main2";
import Bottom from "./components/Bottom";

export default {
  components: {
    Main2,
    Bottom
  },

}
</script>

<style scoped>
  .app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
  h1 {
    color: red;
  }
</style>
