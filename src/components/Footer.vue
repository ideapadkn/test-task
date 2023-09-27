<script setup>
import { ref } from 'vue'

const visible = ref(true)

const hide = () => {
  visible.value = false
}
</script>
<template>
  <div>
    <div v-if="visible" class="footer">
      <div class="footer__content">

      </div>
      <div class="footer__close">
        <button class="btn" @click="hide()">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24px" height="24px">
            <path
              d="M 4.7070312 3.2929688 L 3.2929688 4.7070312 L 10.585938 12 L 3.2929688 19.292969 L 4.7070312 20.707031 L 12 13.414062 L 19.292969 20.707031 L 20.707031 19.292969 L 13.414062 12 L 20.707031 4.7070312 L 19.292969 3.2929688 L 12 10.585938 L 4.7070312 3.2929688 z" />
          </svg>
        </button>
      </div>
    </div>
  </div>
</template>


<style lang="scss" scoped>
.footer {
  display: flex;
  align-items: center;
  padding: 0 18px;
  position: relative;
  background-color: rgba(38, 38, 38, 1);
  border-radius: 12px;
  height: 72px;

  &__content {
    background-color: rgba(77, 77, 77, 1);
    border-radius: 12px;
    height: 36px;
    width: 699px;
  }

  &__close {
    position: absolute;
    top: 10px;
    right: 10px;

    .btn {
      border: none;
      background-color: transparent;
      cursor: pointer;

    }

    svg {
      color: #ffffff;
    }
  }
}</style>