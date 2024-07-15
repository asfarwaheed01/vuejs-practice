<template>
  <h1 class="text-red">Global Styling</h1>
  <p class="text-red">Trying Local scope in this component.</p>
</template>

<!-- Global Style -->
<!-- to make it local just component specific you have to use the work scoped with the style tag -->
<style scoped>
.text-red {
  color: red;
}
</style>
