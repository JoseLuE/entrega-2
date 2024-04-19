<template>
  <div>
    <p>Ancho: {{ state.width }}</p>
    <p>Alto: {{ state.height }}</p>
    <p>Area: {{ area }}</p>
  </div>
</template>

<script>
import { reactive, computed } from 'vue';

export default {
  setup() {
    const state = reactive({
      width: 10,
      height: 5
    });

    const area = computed(() => {
      return state.width * state.height;
    });

    return {
      state,
      area
    };
  }
};
</script>


