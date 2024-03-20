<template>
  <h1>Projet vue</h1>
  <button @click="onClick">J'ai cliqué {{ click }} fois</button>
</template>
<script setup>
import { ref } from "vue";

const click = ref(0);
function onClick() {
  click.value++;
}
</script>

<style>
h1 {
  color: red;
}
button {
  background-color: blue;
  color: white;
  padding: 10px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}
</style>
