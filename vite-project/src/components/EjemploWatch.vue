<template>
    <div>
      <p>Ancho: {{ state.width }}</p>
      <button @click="increaseWidth">Aumetar ancho</button>
    </div>
  </template>
  
  <script>
  import { reactive, watch } from 'vue';
  
  export default {
    setup() {
      const state = reactive({
        width: 10
      });
  
      watchWidth(state);
  
      const increaseWidth = () => {
        state.width++;
      };
  
      return {
        state,
        increaseWidth
      };
    }
  };
  
  function watchWidth(state) {
    watch(() => state.width, (newWidth, oldWidth) => {
      console.log(`El acho cambio de ${oldWidth} a ${newWidth}`);
    });
  }
  </script>
  
  
  