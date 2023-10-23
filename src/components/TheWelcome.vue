<script setup>
import { ref } from 'vue'

const count = ref(0)
</script>

<template>
<main>
  <div class="home">
    <h1>Count</h1>
    <button @click="count++">+</button>
    <span>{{ count }}</span>
    <button @click="count--">-</button>
  </div>
</main>
</template>

<style>
@media (min-width: 1024px) {
  .home {
    min-height: 100vh;
    display: flex;
    justify-items: center;
    align-items: center;
  }
}
</style>