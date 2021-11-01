<template>
  <div class="about">
    <h2>{{ store.state.counter }}</h2>
    <h1>Show Counter as global value</h1>
  </div>
</template>

<script>
import { inject } from 'vue'
export default {
  setup() {
    const store = inject('store')

    return {
      store
    }
  }
}
</script>