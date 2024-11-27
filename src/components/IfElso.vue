<template>
  <h1 v-if="loginStatus">da login</h1>
  <h1 v-else> chua login</h1>

  <button @click="handleToggle">{{ loginStatus ? "logout" : "login" }}</button>

  </template>
  
  <script>
  export default {
    data() {
      return {
        loginStatus: true, 
      };
    },
    methods: {
        handleToggle() {
            this.loginStatus = !this.loginStatus
        }
    }
  };
  </script>
  