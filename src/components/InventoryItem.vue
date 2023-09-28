<script setup>
import { ref } from 'vue'

const figures = ref([
  'green',
  'yellow',
  'blue',
  'black',
  'white',
])
</script>

<template>
  <div>
    <div class="inventory__item">
      <div v-for="figure in figures" :key="figure.id" class="inventory__item-content">
        <ul class="ul">
          <li class="inventory__item-content-item">
            {{ figure }}
          </li>
        </ul>
        <!-- <div class="inventory__item-content-id">
          {{ figure.id }}
        </div> -->
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.inventory__item {
  border: 1px solid rgba(77, 77, 77, 1);
  width: 105px;
  height: 100px;

  &-content {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100px;
    position: relative;

    .ul {
      list-style: none;

    }
    &-item {
      display: flex;
    }

    &-id {
      padding: 2px;
      position: absolute;
      right: 0;
      bottom: 0;
      border: 1px solid rgba(77, 77, 77, 1);
      border-top-left-radius: 12px;
      color: rgba(77, 77, 77, 1);
    }
  }
}
</style>