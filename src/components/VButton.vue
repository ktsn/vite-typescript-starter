<template>
  <button
    class="py-2 px-4 rounded bg-green-500 hover:bg-green-400 text-white transition duration-200 ease-out"
    v-bind="$attrs"
  >
    <slot />
  </button>
</template>

<script lang="ts">
import { Vue, Options } from 'vue-class-component'

class VButton extends Vue {}

export default Options({
  name: 'VButton',
  inheritAttrs: false,
})(VButton)
</script>
