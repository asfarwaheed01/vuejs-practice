<!-- Reactive function cannot accept primitive data types i.e: number, string, boolean -->
<!-- Reactive function is used to create reactive objects -->
<script setup>
import { reactive } from 'vue'
let initialState = reactive({ val: { count: 0 }, user: ['Asfar', 'Ali'] })

const changeUser = () => {
  initialState.user[0] = 'Asjad'
  initialState.user[1] = 'Ahmad'
}
</script>
<template>
  <h1>Current Count:{{ initialState.val.count }}</h1>
  <h2>Users: {{ initialState.user }}</h2>

  <button @click="initialState.val.count += 10">Add 10</button>
  <button @click="changeUser">Change User</button>
  <button @click="initialState.user.push('Haider')">Add one more</button>
</template>
