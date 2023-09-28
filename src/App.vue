<script setup>
// import { RouterView } from 'vue-router'
import draggable from 'vuedraggable'
import { ref } from 'vue'
const meals = ref([
  'Hamburger',
  'Pizza',
  'Tacos',
  'Chiken',
])
</script>

<template>
  <!-- <RouterView /> -->
  <div class="text-white">
    <h1 class="text-3xl mb-5 font-semibold">Meals</h1>
    <draggable v-model="meals" tag="ul">
      <template #item="{ element: meal }">
        <li>{{ meal }}</li>
      </template>
    </draggable>
  </div>
</template>
