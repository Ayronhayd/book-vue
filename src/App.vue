<template>
 <h2>{{title}}</h2>
 <p>{{ message }}</p>
</template>

<script>

export default {
  data() {
    return {
      message: 'Hello Vue!',
      title: 'My First Vue App'
    }
  }
}

</script>

<style scoped>
h2 {
  color: red;
  font-size: 50px;
  text-align: center;
font-family: arial;
}

p {
  color: green;
  font-size: 30px;
  text-align: center;
}

</style>
