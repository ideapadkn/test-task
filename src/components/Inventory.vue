<script setup>
import InventoryItem from './InventoryItem.vue';
import { ref } from 'vue'
const items = ref([])
</script>

<template>
  <div>
    <div class="inventory">
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
      <InventoryItem />
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