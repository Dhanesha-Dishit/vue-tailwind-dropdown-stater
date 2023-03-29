<template>
  <div class="prose max-w-none">
    <h1>{{ msg }}</h1>
    <drop-down />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import DropDown from './DropDown.vue'

export default defineComponent({
  components: { DropDown },
  props: {
    msg: {
      type: String,
      default: '',
    },
  },
})
</script>

<style>
.prose a {
  @apply text-gray-900 underline content-center  !important;
}
</style>
