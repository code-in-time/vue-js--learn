<template>
  <div id="MyTest">
    <button v-on:click="toggle">show / hide button</button>
    this is  test show 
    <div>show: {{show}}</div>
    <h1>{{ title }}</h1>
    
    <p v-show="show" class="toggleClass">show me</p>
        <p v-if="show" class="toggleClass">show me remove from dom</p>
    <p>always visible</p>
    <ul>
      <li v-for="x in persons">{{ x.name }} - {{ x.age }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'MyShowHide',
  data: () =>( {
    show: true,
    persons: [
      { name: 'max', age: 27 },
      { name: 'harry', age: 90 },
      { name: 'fred', age: 8 },
    ],
    title: 'my text',
  }),
  methods: {
    toggle (e) {
      this.show = !this.show;
      
    }
  },
  // computed: {
  //   titleU: () => this.title.toUpperCase()
  // }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.toggleClass {
  color: #42b983;
  background: red;
} 
</style>
