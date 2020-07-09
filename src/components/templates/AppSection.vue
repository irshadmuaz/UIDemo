<template>
    <div class="AppSection">
        <slot/>
    </div>
</template>

<script>
export default {
  name: 'AppSection',
};
</script>

<style>
    .AppSection {
        box-shadow: inset 0 0 2px #000000;
        border-radius: 10px;
        padding: 20px;
    }
</style>
