<!-- We need to make the count a reactive component in order to make it editable -->
<!-- Reactivity is the way by which a framework can automatically change UI if the data behind it changes -->
<script setup>
import { ref } from 'vue'

let count = ref(0)

const Increment = () => {
  count.value++
}
const Decrement = () => {
  count.value--
}
</script>
<template>
  <h1>Count: {{ count }}</h1>
  <button v-on:click="Increment">Increment</button>
  <button @:click="Decrement">Decrement</button>
</template>
