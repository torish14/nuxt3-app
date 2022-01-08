<template>
  <div>
    <h1>{{ title }}</h1>
    <button @click="increment">+</button>
    <p>{{ count }}</p>
    <button @click="decrement">-</button>
  </div>
</template>

<script setup lang="ts">
const title = 'Nuxt3'
let count = ref(0)

const increment = () => count.value++
const decrement = () => count.value--
</script>
