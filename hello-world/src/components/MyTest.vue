<template>
  <div id="MyTest">
    <button v-on:click="increment">increment</button>
    this is  test
    <p>Counter: {{ counter }}</p>
    <p>Clicks: {{ clicks }}</p>
  </div>
</template>

<script>
export default {
  name: 'MyTest',
  data: () =>( {
    counter: 0,
    clicks: 0
  }),
  methods: {
    increment (e) {
      console.log('el',e);
     // alert('test');
      this.counter  = this.counter + 2;
      this.clicks++;
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* h3 {
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
} */
</style>
