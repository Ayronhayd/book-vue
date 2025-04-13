<template>

  <input type="login" v-model="userName" />
  <br>
  <input type="password"  v-model="userPassword"/>
  <br>
  <input type="email" v-model="userEmail" />
  <br />
  <button type="button" @click="userData()">{{ btn }}</button>





  <div>
    {{ users }}
    <button type="button" @click="users = []">Удалить</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      users: [],
      btn: 'Отправить',
      userName: '',
      userPassword: '',
      userEmail: '',
    }
  },
  methods: {
    userData() {
      this.btn = 'Ок'
      this.users.push({
        userName: this.userName,
        userPassword: this.userPassword,
        userEmail: this.userEmail,
      })
    },
  },
}
</script>

<style scoped>
* {
  margin: 0 0 0 10px;
  padding: 10px;
}

h2 {
  color: red;
  font-size: 50px;
}

p {
  color: green;
  font-size: 30px;
}
</style>
