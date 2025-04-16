<template>
  <h1> Счетчик {{ counter }}  {{ counter }}</h1>

  <span className="cpap" v-bind:title="massage">Подсказка</span>
</template>

<script>

export default {

  data() {
  return {
    counter: 0,
    massage: 'Hello'
  }
  },
  mounted() {
    setInterval(() => {
      this.counter++
    }, 1000)
  }
}

</script>

<style scoped>
.cpap {
  color: red
}

* {
  margin: 0 0 0 10px;
  padding: 10px;
}
</style>
