<script setup>
import Footer from '../components/Footer.vue';
import Menu from '../components/Menu.vue';
import Inventory from '../components/Inventory.vue';
</script>

<template>
  <div>
    <div class="main">
      <div class="main__content">
        <Menu />
        <Inventory />
      </div>
    </div>
    <Footer />
  </div>
</template>

<style lang="scss" scoped>
  .main {
    &__content {
      display: flex;
      align-items: center;
      gap: 24px;
    }
  }
</style>
