<template>
 <h2>{{title}}</h2>
 <p>{{ message }}</p>


 <button type="button" @click="userData()">{{ btn}}</button>

<div class="wrap">
<input type="text" v-model="text">

<p>{{ text }}</p>
</div>

</template>

<script>


export default {
  data() {
    return {
      message: 'Hello Vue!',
      title: 'My First Vue App',
      btn: 'Отправить',
      text: ''
    }
  },
  methods: {
    userData() {
      this.title= 'New title'
      this.message= 'New message'
      this.btn= 'New button'

    }
  }
}

</script>

<style scoped>
* {
  margin: 30px;
  padding: 30px;
}



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
