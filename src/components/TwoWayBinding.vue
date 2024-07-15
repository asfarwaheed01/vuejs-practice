<script setup>
import { ref } from 'vue'
const formData = ref({ username: '', email: '', password: '' })
</script>
<template>
  <div>
    <form @submit.prevent>
      <input type="text" placeholder="enter your name" v-model="formData.username" />
      <input type="text" placeholder="enter your email" v-model="formData.email" />
      <input type="text" placeholder="enter your password" v-model="formData.password" />
      <button type="submit">Submit</button>
    </form>

    <p>{{ formData.username }}</p>
    <p>{{ formData.password }}</p>
    <p>{{ formData.email }}</p>
  </div>
</template>
