<script setup>
import { ref } from 'vue';
import {parseSql} from '../utils/parse'
// Déclarez une variable réactive pour stocker la valeur de la zone de texte
const sqlInput = ref('');
const parse = () => {
    parseSql(sqlInput.value)
}
</script>

<template>
  <div class="flex flex-row w-1/2">
    <!-- Utilisez v-model pour lier la valeur de la zone de texte à sqlInput -->
    <textarea v-model="sqlInput" placeholder="Enter SQL here" class="w-96"></textarea>
  </div>
  <!-- Ajoutez un gestionnaire d'événements @click pour appeler parseSql lorsque le bouton est cliqué -->
  <button @click="parse" class="bg-blue-900 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
    Submit
  </button>
</template>

<style scoped>
</style>
