<template>
  <h1>This is a Form</h1>
  <form @submit="submitHandler">
    <input type="text" v-model="name" placeholder="Please Enter your name" />
    <input type="email" v-model="email" placeholder="Please Enter your email" />
    <button type="submit">Submit</button>
  </form>
</template>

<script setup>
import { ref } from 'vue'

let name = ref('')
let email = ref('')

const submitHandler = (e) => {
  e.preventDefault()
  console.log('Name:', name.value)
  console.log('Email:', email.value)
  alert('Valid Credentials')
}
</script>
