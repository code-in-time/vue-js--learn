<template>
    <div>
        <input type="text" :value="msg"  @input="changeMessage" >
        <div>this is test input text: {{ message }}</div>
    </div>
</template>

<script>
  export default {
    props: ['msg'],
    data: () => {
      return {
        message: 0
      };
    },
    methods: {
      changeMessage(e) {
        //console.log('message', e.target.value)
        this.message =  e.target.value;
        this.$emit('myMessageChanged', this.message );
      },
    }
};
</script>

