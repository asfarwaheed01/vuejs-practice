<script setup>
const myName = 'Asfar Waheed'
const myNumber = '03174400231'
function Add(x, y) {
  return x + y
}

// Attribute Binding
const Link = 'https://www.google.com'
const Image =
  'https://images.unsplash.com/photo-1719216323699-79e62fbc6a56?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90b3MtZmVlZHw2fHx8ZW58MHx8fHx8'
const imageWidth = 400
const imageHeight = 400

// Dynamic Binding
const imageInfo = {
  src: 'https://images.unsplash.com/photo-1718905147097-418b73c620bb?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90b3MtZmVlZHwyN3x8fGVufDB8fHx8fA%3D%3D',
  alt: 'Image Text',
  width: 400,
  height: 400
}
</script>

<template>
  <div>
    <h2>Hello my name is {{ myName }}</h2>
    <h2>My Contact Number is {{ myNumber }}</h2>
    <h2>The Addition is: {{ Add(2, 2) }}</h2>
    <!-- <a v-bind:href="Link">Google</a> -->
    <a :href="Link">Google</a>
    <img v-bind:src="Image" :alt="Image" :width="imageWidth" :height="imageHeight" />
    <img :="imageInfo" />
  </div>
</template>
