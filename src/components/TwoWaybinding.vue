<template>
    <div>
      <input type="checkbox" v-model="arrayOne" value="Monday" id="Monday">
      <label for="Monday">Monday</label>
  
      <input type="checkbox" v-model="arrayOne" value="friday" id="friday">
      <label for="friday">friday</label>
  
      <p>{{ arrayOne }}</p> 
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        arrayOne: [], 
      };
    },
  };
  </script>
  