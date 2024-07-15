<script setup>
import { ref } from 'vue'
const count = ref(0)
let username = ref('')
const userList = ref(['user 1', 'user 2', 'user 3'])
</script>
<template>
  <h1>Count is:{{ count }}</h1>
  <h1>Username: {{ username }}</h1>
  <button @:click="count++">+</button>
  <button @:click="count--">-</button>
  <button @:click="username = 'Asfar'">Set Username</button>

  <div class="list">
    <div v-for="(user, index) in userList" :key="index">
      {{ user }}
    </div>
  </div>
</template>

<style scoped>
.list {
  display: flex;
  gap: 5px;
  margin-top: 10px;
}
</style>
