<script setup lang="ts">
  import { RouterView } from 'vue-router'
  import { Header, Footer } from '@/components/main'
  import { Navigation } from '@/components/navigation'

</script>

<template>
  <Header />

  <Navigation />

  <section class="tw-body container">
    <RouterView />
  </section>

  <Footer />
</template>

<style lang="scss">

  @import '@/assets/scss/constants';
  @import '@/assets/scss/links';

  .tw-body {
    margin-top: 1.5rem;
    min-height: $default-body-height;
    padding-top: 0.5rem;
    padding-bottom: 0.5rem;
  }
</style>
