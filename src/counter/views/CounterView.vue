<script setup lang="ts">
import { ref } from 'vue'

const counter = ref(0)

const incrase = () => {
  if (counter.value !== 10) {
    counter.value++
  } else {
    counter.value = 0
  }
}
</script>

<template>
  <h1>Contador View: {{ counter }}</h1>
  <button @click="incrase">+1</button>
</template>

<style scoped></style>
