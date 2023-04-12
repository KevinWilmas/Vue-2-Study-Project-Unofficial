<template>
    <div>
      <input type="text" v-model="name" />
    </div>
  </template>
  
  <script>
  import { ref, watchEffect } from "vue";
  export default {
    setup() {
      const name = ref('');
      watchEffect(() => {
        console.log(name.value);
      })
      return { name };
    }
  };
  </script>
