<script setup>
import HelloWorld from './components/HelloWorld.vue'
import SqlInput from './components/SqlInput.vue';
</script>

<template>
  <div class="m-20 w-full">
    <h1 class=" font-bold text-4xl text-center ">
    SQL VISUALIZER
    </h1>
    <SqlInput/>
  </div>

  
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
