<template>
  <div id="MyTest">
    <button v-on:click="toggle">show / hide button</button>
    this is  test show 
    <div>show: {{show}}</div>
    
    <p v-show="show" class="toggleClass">show me</p>
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
    ]
  }),
  methods: {
    toggle (e) {
      this.show = !this.show;
      
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.toggleClass {
  color: #42b983;
  background: red;
} 
</style>
