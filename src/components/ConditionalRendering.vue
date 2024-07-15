<script setup>
import { ref } from 'vue'
const isTrue = false
let isFalse = false

const isVisible = ref(true)
</script>
<template>
  <div>
    <p v-if="isTrue">This will show only when isTrue is true.</p>
    <p v-else-if="isFalse">This will show only when isFalse is true.</p>
    <p v-else>This will show only when no condition is true.</p>
    <p v-show="isVisible">This will be shown or not based on the value of isVisible.</p>
    <button @click="isVisible = !isVisible">Toggle Visibility</button>
  </div>
</template>
