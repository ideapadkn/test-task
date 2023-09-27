<script setup>
import Footer from '../components/Footer.vue';
import Menu from '../components/Menu.vue';
import Inventory from '../components/Inventory.vue';
</script>

<template>
  <div class="container">
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
  margin-bottom: 24px;

  &__content {
    display: flex;
    gap: 24px;
  }
}
</style>
