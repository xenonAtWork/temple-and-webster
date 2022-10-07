<script setup lang="ts">
  import { RouterLink } from 'vue-router'

</script>

<template>
  <div class="tw-main-logo-placeholder">
    <div class="tw-main-logo">
      <RouterLink to="/">
        <img alt="TW Logo" src="https://img.zcdn.com.au/st4/stores/common/logos/temple_&_webster/temple_&_webster_normal_1_default_background.svg?v=2" />
      </RouterLink>
    </div>
  </div>
</template>

<style lang="scss" scoped>

  @import '@/assets/scss/tw-theme';
  @import '@/assets/scss/constants';

  .tw-main-logo-placeholder {
    height: $default-header-height;
    width: calc($default-header-logo-width + ($default-header-logo-padding * 2) + ($default-header-logo-border-width * 2));
    position: relative;
    
    .tw-main-logo {
      background-color: $white-color;
      border: $default-header-logo-border-width solid $layout-color;
      border-bottom-left-radius: 0.5rem;
      border-bottom-right-radius: 1rem;

      padding: $default-header-logo-padding;
      position: absolute;

      &:hover {
        box-shadow: rgba(0, 0, 0, 0.1) 0px 10px 50px;
      }

      img {
        width: $default-header-logo-width;
      }
    }
  }
</style>