<template>
  <article class="p-5">
    <h1 class="text-green-800 text-3xl font-bold">Hello Vite + Vue 3!</h1>
    <p>Edit ./App.vue to test hot module replacement (HMR).</p>
    <p class="mt-2">
      <span class="block">Count is: {{ count }}</span>
      <VButton @click="count++">increment</VButton>
    </p>
  </article>
</template>

<script lang="ts">
import { Vue, Options } from 'vue-class-component'
import VButton from './components/VButton.vue'

class App extends Vue {
  count = 0
}

export default Options({
  components: {
    VButton,
  },
})(App)
</script>
