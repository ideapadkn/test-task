<script setup>
import InventoryItem from './InventoryItem.vue';
</script>

<template>
  <div>
    <div class="inventory">
      <InventoryItem v-for="(item, index) of new Array(25)" :key="index" />
    </div>
  </div>
</template>


<style lang="scss" scoped>
.inventory {
  display: flex;
  flex-wrap: wrap;
  background-color: rgba(38, 38, 38, 1);
  border-radius: 12px;
  height: 500px;
  overflow: hidden;
  border: 1px solid rgba(77, 77, 77, 1);
}
</style>