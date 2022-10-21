<script setup lang="ts">

  defineProps<{
    navItemLink: string,
    navItemText: string
  }>()

</script>

<template>
  <div class="item">
    <a :href="navItemLink" class="clean-link">{{ navItemText }}</a>
  </div>
</template>

<style lang="scss" scoped>

  @import '@/assets/scss/constants';

  .item {
    font-size: $font-14;
    min-width: 3rem;
    padding: 0.5rem 1.5rem;
  }
</style>
