<template>
  <app-section class="AppForm">
    <form>
      <div :class="inline ? 'inline':'ninline'" v-for="(formItem, key) in formData" :key="key">
        <label class="AppLabelForm" :for="formItem.name">{{formItem.label}}</label>
        <app-select v-if="formItem.fieldType === 'AppSelect'"
         :options="formItem.options"></app-select>
        <app-input v-else-if="formItem.fieldType === 'AppInput'"></app-input>
      </div>
      <div :class="inline ? 'inline':'ninline'">
        <app-button>{{buttonText}}</app-button>
      </div>
      <slot />
    </form>
  </app-section>
</template>

<script>
import atoms from '../atoms';
import templates from '../templates';

export default {
  components: {
    ...atoms,
    ...templates,
  },

  props: {
    formData: {
      type: Array,
      default: () => [],
    },
    inline: {
      type: Boolean,
      default: false,
    },
    buttonText: {
      type: String,
      default: 'Submit',
    },
  },
};
</script>

<style scoped>
 .ninline {
     padding: 5px;
     width: 200px;
 }
 .inline {
     padding: 20px;
     display: inline-block;
     width: 200px;
 }
 .AppForm {
     text-align: left;
 }
 .AppLabelForm {
     width: 100px;
     display: block;
     font-family: tahoma;
     margin-bottom: 5px;
     font-size: small;
 }
</style>
