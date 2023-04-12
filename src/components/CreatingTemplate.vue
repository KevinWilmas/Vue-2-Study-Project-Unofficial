<template>
    <div class="form-element">
      <h2>{{ title }}</h2>
      <input type="text" v-model="username" placeholder="Username" />
  
      <input type="password" v-model="password" placeholder="Password" />
  
      <button @click="login">Submit</button>
      <p>Values: {{ username + ' ' + password }}</p>
    </div>
  </template>
  
  