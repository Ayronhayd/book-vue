<script setup>
import { ref } from 'vue';

const city = ref("Топ 1")


</script>

<template>
<div className="wrapp">
  <h1>Погодное приложения {{ city }}</h1>
  <p>Узнать погоду в вашем городе</p>
  <input className="text-pass" type="text" placeholder="Введите город">
  <button className="btn">Узнать</button>
</div>


</template>

<style>
.wrapp {
width: 500px;
height: 300px;
margin: 0 auto;
background-color: rgba(211, 214, 13, 0.767);
border-radius: 12px;
padding: 20px;
text-align: center;
}
h1 {
  color: rgb(235, 41, 6);
}

p {
color: blueviolet;
}

.text-pass {
  padding: 10px;
  color: rgb(14, 153, 9);
}

.text-pass::placeholder{
  color: red;
}

.btn {
  padding: 10px;
  margin-left: 10px;
}

</style>
