<script setup>
import { ref, onMounted } from 'vue';
const contador = ref(0)

function incrementarContador() {contador.value++}
function decrementarContador() {if (contador.value > 0){contador.value-- }

}
</script>

<template>
  <button @click="incrementarContador">Incrementar</button>
  <button @click="decrementarContador">Decrementar</button>
  <p>O valor do contador é: {{ contador }}</p>
</template>

<style scoped>
button {
  font-weight: bold;
}
</style>
