<template>
  <div>
    <div v-if="show"><slot></slot></div>
  </div>
</template>

<script>
function processamentoIntenso() {
  let resultado = 0
  for (let i = 0; i < 100000000; i++) {
    resultado += Math.sqrt(i)
  }
  return resultado
}

export default {
  data() {
    return { show: false }
  },

  mounted() {
    processamentoIntenso()
    this.show = true
  },
}
</script>
