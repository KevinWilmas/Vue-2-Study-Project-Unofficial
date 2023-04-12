<template>
  <div class="form-element">
    <h2>{{ state.title }}</h2>
    <input type="text" v-model="state.username" placeholder="Username" />
    <input type="password" v-model="state.password" placeholder="Password" />
    <button @click="login">Submit</button>
    <p>Values: {{ state.username + ' ' + state.password }}</p>
  </div>
</template>
  