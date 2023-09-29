<script setup>
import { ref } from 'vue'

const items = ref([
  { id: 0, title: 'Item 1', list: 1 },
  { id: 1, title: 'Item 2', list: 2 },
  { id: 2, title: 'Item 3', list: 3 },
])

const getList = (list) => {
  return items.value.filter((item) => item.list == list)
}

const startDrag = (event, item) => {
  console.log(item);
  event.dataTransfer.dropEffect = 'move'
  event.dataTransfer.effectAllowed = 'move'
  event.dataTransfer.setData('itemID', item.id)
}

const onDrop = (event, list) => {
  const itemID = event.dataTransfer.getData('itemID')
  const item = items.value.find((item => item.id == itemID))
  item.list = list
}
</script>

<template>
  <div class="drop__zone" @drop="onDrop($event, 1)" @dragenter.prevent @dragover.prevent>
    <div class="drop__zone-el" v-for="item in getList(1)" :key="item.id" draggable="true"
      @dragstart="startDrag($event, item)">
      {{ item.title }}
    </div>
  </div>
  <div class="drop__zone" @drop="onDrop($event, 2)" @dragenter.prevent @dragover.prevent>
    <div class="drop__zone-el" v-for="item in getList(2)" :key="item.id" draggable="true"
      @dragstart="startDrag($event, item)">
      {{ item.title }}
    </div>
  </div>
  <div class="drop__zone" @drop="onDrop($event, 3)" @dragenter.prevent @dragover.prevent>
    <div class="drop__zone-el" v-for="item in getList(3)" :key="item.id" draggable="true"
      @dragstart="startDrag($event, item)">
      {{ item.title }}
    </div>
  </div>
</template>

<style lang="scss" scoped>
.drop__zone {
  border: 1px solid rgba(77, 77, 77, 1);
  height: 100px;
  width: 105px;

  &-el {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100px;
    width: 105px;
    cursor: pointer;
    color: #fff;
  }
}
</style>