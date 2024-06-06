<script setup>
import { ref } from 'vue'
import Button from './Button'

const count = ref(0);

const increment = () => {
  count.value++
}

const decrement = () => {
  count.value--
}
</script>

<template>
  <div class="Counter-container">
    <h2>Counter: {{ count }}</h2>
    <div class="Counter-button-row">
      <Button
      :action="increment"
      label="+1" />
    <Button
      :action="decrement"
      label="-1" />
    </div>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Tiny5&display=swap');

.Counter-container {
  font-family: "Tiny5", sans-serif;
  font-weight: 400;
  font-style: normal;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 1rem;
  background-color: #444;
  color: snow;
}

.Counter-button-row {
  margin-top: 20px;
  display: flex;
  flex-direction: row;
  gap: 8px;
}
</style>