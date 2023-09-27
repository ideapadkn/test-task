<script setup>
import InventoryItem from './InventoryItem.vue';
import { ref } from 'vue'
const items = ref([])


</script>

<template>
  <div class="container">
    <div class="inventory">
      <InventoryItem v-for="item in items" :key="item.id" />
    </div>
  </div>
</template>


<style lang="scss" scoped>
.inventory {
  border-radius: 12px;
  background-color: rgba(38, 38, 38, 1);
  width: 525px;
  height: 500px;
}
</style>