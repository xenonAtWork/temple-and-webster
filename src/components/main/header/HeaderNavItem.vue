<script setup lang="ts">
</script>

<template>
  <div class="item">
    <span class="item-icon">
      <slot name="icon"></slot>
    </span>
    <span class="item-text">
      <slot></slot>
    </span>
  </div>
</template>

<style lang="scss">

  @import '@/assets/scss/mixins';
  @import '@/assets/scss/constants';
  @import '@/assets/scss/tw-theme';

  .item {
    @include flexbox();
    @include flex_align_items(center);
    cursor: pointer;
    color: $darker-primary-color;
    padding: 0 1rem;
    
    &:hover {
      background-color: $primary-color;
      filter: brightness(0.90);
    }

    .item-icon {
      font-size: $default-header-nav-icon-size;
    }

    .item-text {
      margin-left: 0.25rem;
    }
  }
</style>
