<template>

<ul>
  <li v-for="number in numbers" :key="number"> {{ number }} </li>
</ul>
</template>

<script>

export default {
  data() {
    return {
      numbers: [1, 2, 3, 4, 5],
    }
  }
}
</script>

<style scoped>
* {
  margin: 0 0 0 10px;
  padding: 10px;
}
</style>
