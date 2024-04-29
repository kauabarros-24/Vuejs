<script>
export default {
  data() {
    return {
      contador: 0
    }
  },
  methods: {
    incrementarContador() {
      this.contador++
    },
    decrementarContador() {
      if (this.contador > 0 ) {
        this.contador--;
      }
      else {
        alert("Contador menor que zero não pode ser decrementado")
      }
    }
  },
  mounted() {
    console.log(`O valor inicial do contador é ${this.contador}.`)
  }
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
