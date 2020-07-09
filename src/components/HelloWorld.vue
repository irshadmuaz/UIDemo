<template>
  <div>
    <h1>Peloton UI Demo</h1>

    <app-form :form-data="formData " :inline="false"></app-form>
  </div>
</template>

<script>
import AppButton from './atoms/AppButton';
import AppInput from './atoms/AppInput';
import AppSelect from './atoms/AppSelect';

import AppForm from './molecules/AppForm'
  ;

export default {
  name: 'HelloWorld',
  data() {
    return {
      msg: 'Welcome to Your Vue.js App',
      options: [{ label: 'Option1', value: 'option1' },
        { label: 'Option1', value: 'option1' },
        { label: 'Option1', value: 'option1' },
        { label: 'Option1', value: 'option1' }],

      formData: [{
        label: 'User Name',
        fieldType: 'AppInput',
      }, {
        label: 'Password',
        fieldType: 'AppInput',
      }, {
        label: 'City',
        fieldType: 'AppSelect',
        options: [
          { label: 'Atlanta', value: 'atlanta' },
          { label: 'Clemson', value: 'clemson' },
          { label: 'Alpharetta', value: 'alpharetta' },
        ],
      }, {
        label: 'Email',
        fieldType: 'AppInput',
      }],

    };
  },
  components: {
    AppButton,
    AppInput,
    AppSelect,
    AppForm,
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
