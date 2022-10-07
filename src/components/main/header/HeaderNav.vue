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

    <span>{{ msg }}</span>
    
    <div class="tw-header-right-nav-items">
      <HeaderNavItem>
        <template #icon>
          <RouterLink to="/about">
            <IconAbout />
          </RouterLink>
        </template>
        <!-- empty nav text -->
      </HeaderNavItem>

      
      <HeaderNavItem>
        <template #icon>
          <IconAccount />
        </template>
        Account
      </HeaderNavItem>

      <HeaderNavItem>
        <template #icon>
          <IconCart />
        </template>
        <!-- empty nav text -->
      </HeaderNavItem>
    </div>
  </nav>
</template>

<style lang="scss" scoped>
  
  @import '@/assets/scss/mixins';

  nav {
    @include flexbox();
    @include flex_align_items(center);
    @include flex_justify_content(space-between);
  }

  .tw-header-right-nav-items {
    @include flexbox(inline-flex);
  }

</style>
