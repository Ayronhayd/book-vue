<script setup>
import { ref } from 'vue'
import ChildComp from './ChildComp.vue'
const greeting = ref('Привет от родителя')
const hoop = ref('Привет от родителя в хуке')
</script>

<template>
  <ChildComp :msg="greeting" :message ="hoop" />


</template>
