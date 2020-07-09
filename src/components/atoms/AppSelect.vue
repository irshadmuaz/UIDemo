<template>
        <select class="AppSelect" name="select" id="select">
            <option v-for="option in options" :key="option.value" :value="option.value">
                {{option.label}}
            </option>
        </select>
</template>

<script>
export default {
  name: 'AppSelect',
  props: {
    label: {
      type: String,
      default: '',
    },
    options: {
      type: Array,
      default: () => [],
    },
  },
};
</script>

<style scoped>
  .AppSelect{
    text-align: left;
    padding:10px;
    border-radius: 5px;
    border: 2px solid gainsboro;
    min-width: 150px;
  }
</style>
