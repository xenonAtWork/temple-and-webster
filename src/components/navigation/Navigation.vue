<script setup lang="ts">
  import { NavigationItem } from '.'

</script>

<template>
  <section class="tw-navigation">
    <div class="container">
      <div class="tw-navigation-items">
        <NavigationItem navItemLink="#" navItemText="Furniture" />
        <NavigationItem navItemLink="#" navItemText="Outdoor" />
        <NavigationItem navItemLink="#" navItemText="Rugs" />
        <NavigationItem navItemLink="#" navItemText="Bed &amp; Bath" />
        <NavigationItem navItemLink="#" navItemText="Lighting" />
        <NavigationItem navItemLink="#" navItemText="Home Décor" />
        <NavigationItem navItemLink="#" navItemText="Office" />
        <NavigationItem navItemLink="#" navItemText="Wall Art" />
        <NavigationItem navItemLink="#" navItemText="Kitchen" />
        <NavigationItem navItemLink="#" navItemText="Baby &amp; Kids" />
        <NavigationItem navItemLink="#" navItemText="Renovation" />
        <NavigationItem navItemLink="#" navItemText="Pet" />
        <NavigationItem navItemLink="#" navItemText="Lifestyle" />
        <NavigationItem navItemLink="#" navItemText="New" />
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>

  @import '@/assets/scss/tw-theme';

  .tw-navigation {
    border-bottom: 1px solid $lightgrey-color;
    box-shadow: rgba(0, 0, 0, 0.1) 0px 0px 50px;
    padding-top: 1.5rem;
    padding-bottom: 0.5rem;
  }
  
  .tw-navigation-items {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
  }
  
</style>
