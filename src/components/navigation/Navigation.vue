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
  
  .tw-navigation-items {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
    margin-top: 1.5rem;
  }
  
</style>
