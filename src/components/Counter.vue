<template>
  <div>{{ count }}</div>
  <button @click="increment">+1</button>
</template>

<script lang="ts">

import { defineComponent, ref } from 'vue'

// properly infer types in typescript
export default defineComponent({
  name: 'Counter',
  setup() {
    const count = ref(0);

    function increment() {
      count.value++;
    }

    return {
      count,
      increment     
    }
  }
});
</script>