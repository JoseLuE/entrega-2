<script setup>
import EjemploRef from './components/EjemploRef.vue';
import EjemploReactivo from './components/EjemploReactivo.vue';
import EjemploComputed from './components/EjemploComputed.vue';
import EjemploWatch from './components/EjemploWatch.vue';
</script>

<template>
  <div id = "#app">
   <h1>Ejemplo ref</h1>
   <EjemploRef/>
   <br>
   <h1>Ejemplo reactivo</h1>
   <EjemploReactivo/>
   <br>
   <h1>Ejemplo computed</h1>
   <EjemploComputed/>
   <br>
   <h1>Ejemplo watch</h1>
   <EjemploWatch/>

  </div>
</template>


