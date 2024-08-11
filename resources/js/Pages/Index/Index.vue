<template>
    <div>Hello!</div>
    <div>Counter: {{ counter }}</div>
  </template>
  
  <script setup>
  import { ref } from 'vue'
  
  const counter = ref(1)
  
  setInterval(() => {
    counter.value++
  }, 1000)
  </script>
  