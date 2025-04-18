<script setup>
import { reactive, ref } from 'vue'

const counter = reactive({ count: 0 })
const message = ref('Привет мир!')
</script>


<template>
  <h1>{{ message }}</h1>
  <p>Количество: {{ counter.count }}</p>
</template>
