<template>
  <div>
    <h1>Peloton UI Demo</h1>
    <app-button>Submit</app-button>
    <app-input></app-input>
    <app-select :options="options"></app-select>
  </div>
</template>

<script>
import AppButton from './atoms/AppButton';
import AppInput from './atoms/AppInput';
import AppSelect from './atoms/AppSelect';

export default {
  name: 'HelloWorld',
  data() {
    return {
      msg: 'Welcome to Your Vue.js App',
      options: [{ label: 'Option1', value: 'option1' },
        { label: 'Option1', value: 'option1' },
        { label: 'Option1', value: 'option1' },
        { label: 'Option1', value: 'option1' }],

    };
  },
  components: {
    AppButton,
    AppInput,
    AppSelect,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
}
</style>
