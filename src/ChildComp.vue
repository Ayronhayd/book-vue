<script setup>




defineProps({
  btn: String
})

</script>

<template>
  <button>{{ btn || 'default' }}</button>

</template>


