<template>
  <div  class="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <h1>test</h1>
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <MyTest />
    <MyShowHide />
    <AppFormInput />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import MyTest from './components/MyTest.vue'
import MyShowHide from './components/myShowHide'
import AppFormInput from './components/AppFormInput'

export default {
  // name: 'appddddddd',
  components: {
    // HelloWorld,
    MyTest,
    MyShowHide,
    AppFormInput
  }
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
