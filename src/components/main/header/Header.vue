<script setup lang="ts">
  import { HeaderNav } from '.'

</script>

<template>
  <section class="tw-header">
    <HeaderNav msg="Welcome, Guest!" />
  </section>
</template>

<style lang="scss" scoped>
  
  @import '@/assets/scss/mixins';
  @import '@/assets/scss/tw-theme';
  @import '@/assets/scss/constants';

  .tw-header {
    background-color: $primary-color;
    height: $default-header-height;
  }

</style>
