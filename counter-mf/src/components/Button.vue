<script setup>
import { toRefs } from 'vue'

const props = defineProps({
  label: String,
  action: Function
})

</script>

<template>
  <button @click="action">{{ label }}</button>
</template>

<style>
</style>