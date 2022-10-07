<script setup lang="ts">
  import { RouterView } from 'vue-router'
  import { Header, Footer } from '@/components/main'
  
</script>

<template>
  <Header />

  <section class="tw-body container">
    <RouterView />
  </section>

  <Footer />
</template>

<style lang="scss" scoped>

  @import '@/assets/scss/constants';

  .tw-body {
    margin-top: 1.5rem;
    min-height: $default-body-height;
    padding-top: 0.5rem;
    padding-bottom: 0.5rem;
  }
</style>
