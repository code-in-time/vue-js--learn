<template>
    <div>
        <input type="text" v-model="myInputText" />
        <div>this is test input text: {{  myInputText }}</div>
    </div>
</template>

<script>
export default {
  name: 'AppFormInput',
  data: () => {
    return {
      myInputText: 0
    };
  }
};
</script>

