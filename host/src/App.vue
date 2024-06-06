<script setup>
import Navbar from "navbar/Navbar"
import Counter from "counter/Counter"
</script>

<template>
  <Navbar />

  <div class="App-container">
    <h3>Contador MF</h3>
    <Counter />
  </div>
</template>

<style scoped>
.App-container {
  margin: 1rem 2.5rem;
}
</style>