<script setup lang="ts">
  import { RouterLink } from 'vue-router'
  import { HeaderLogo, HeaderNavItem } from '.'
  import {
    IconAbout, IconAccount, IconCart 
  } from './icons'

  defineProps<{
    msg: string
  }>()
</script>

<template>
  <nav class="container">
    <HeaderLogo />

    <span class="tw-header-welcome-msg">{{ msg }}</span>
    
    <div class="tw-header-right-nav-items">

      <RouterLink to="/about">
        <HeaderNavItem>
          <template #icon>
            <IconAbout />
          </template>
          <!-- empty nav text -->
        </HeaderNavItem>
      </RouterLink>

      <RouterLink to="/account">
        <HeaderNavItem>
          <template #icon>
            <IconAccount />
          </template>
          Account
        </HeaderNavItem>
      </RouterLink>

      <RouterLink to="/cart">
        <HeaderNavItem>
          <template #icon>
            <IconCart />
          </template>
          <!-- empty nav text -->
        </HeaderNavItem>
      </RouterLink>
    </div>
  </nav>
</template>

<style lang="scss" scoped>
  
  @import '@/assets/scss/mixins';
  @import '@/assets/scss/tw-theme';

  nav {
    @include flexbox();
    @include flex_align_items(center);
    @include flex_justify_content(space-between);
  }

  .tw-header-welcome-msg {
    color: $white-color;
  }

  .tw-header-right-nav-items {
    @include flexbox(inline-flex);

      a {
        color: inherit;
        text-decoration: none;
      }
  }

</style>
