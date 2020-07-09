<template>
        <input class="AppInput" type="text">
</template>

<script>
export default {
  name: 'AppInput',
  props: {
  },
};
</script>

<style scoped>
  .AppInput{
    text-align: left;
    padding:10px;
    border-radius: 5px;
    border: 1px solid gainsboro;
    min-width: 200px;
  }
</style>
