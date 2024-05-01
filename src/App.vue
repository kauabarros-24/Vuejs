<script>
export default {
  data() {
    return {
      nome: "Kaua",
      idade: 16,
      contador: 0

    }
  },
  methods: {
    inverterTexto(texto) {
      return texto.split('').reverse().join('')
    } 
  }
}
</script>

<template>
  <p v-if="contador > 10">O contador é maior que 10</p>
  <p v-if="contador < 10">O contador é menor que 10</p>
  <p>{{ contador }}</p>
  <p>{{ inverterTexto(nome) }}</p>

</template>

<style scoped>
p {
  font-weight: bold;
}
</style>
