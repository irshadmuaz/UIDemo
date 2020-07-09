<template>
    <button class="AppButton" @click="click">
        <slot/>
    </button>
</template>

<script>
export default {
  name: 'AppButton',
  props: {

  },
  methods: {
    buttonClick() {
      this.$emit('click');
    },
  },
};
</script>

<style scoped>
  .AppButton{
    border-radius: 5px;
    border-top-left-radius: 20px;
    border-bottom-left-radius: 20px;
    border-top-right-radius: 20px;
    border-bottom-right-radius: 20px;
    width:150px;
    padding: 10px;
    border: 1px solid gainsboro
  }
</style>
