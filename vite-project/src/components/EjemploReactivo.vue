<template>
    <div>
      <p>Name: {{ state.name }}</p>
      <button @click="updateName">Cambiar el nombre</button>
    </div>
  </template>
  
  <script>
  import { reactive } from 'vue';
  
  export default {
    setup() {
      const state = reactive({
        name: 'Ivan'
      });
  
      const updateName = () => {
        state.name = 'Jaime';
      };
  
      return {
        state,
        updateName
      };
    }
  };
  </script>
  