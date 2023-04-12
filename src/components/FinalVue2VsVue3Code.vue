<template>
    <div class="form-element">
      <h2>{{ title }}</h2>
      <input type="text" v-model="username" placeholder="Username" />
  
      <input type="password" v-model="password" placeholder="Password" />
  
      <button @click="login">Submit</button>
      <p>Values: {{ username + ' ' + password }}</p>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      title: String,
    },
    data() {
      return {
        username: '',
        password: '',
      }
    },
    mounted() {
      console.log('title: ' + this.title)
    },
    computed: {
      lowerCaseUsername() {
        return this.username.toLowerCase()
      },
    },
    methods: {
      login() {
        this.$emit('login', {
          username: this.username,
          password: this.password,
        })
      },
    },
  }
  </script>
  