<script setup>
import { reactive, ref } from 'vue'

const counter = reactive({ count: 0 })

defineProps({
  msg: String,
  message: String
})

</script>

<template>
  <h1>{{ message }}</h1>
  <p>Количество: {{ counter.count }}</p>

  <h2>{{ msg || 'пока входные параметры не переданы' }}</h2>
</template>


