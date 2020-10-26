<template>
  <HelloWorld msg="composition API test"/>
  <Counter/>
</template>

<script>
import HelloWorld from '@/components/HelloWorld.vue'
import Counter from '@/components/Counter.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Counter
  }
}
</script>
