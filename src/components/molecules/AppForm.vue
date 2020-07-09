<template>
    <app-section>
        <form>
            <slot/>
        </form>
    </app-section>
</template>

<script>
import { AppSelect, AppInput, AppButton } from '../atoms';
import { AppSection } from '../templates';

export default {
  components: {
    AppSection,
    AppInput,
    AppSelect,
    AppButton,
  },


};
</script>
