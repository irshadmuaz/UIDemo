<template>
    <button @click="click">
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

</style>
