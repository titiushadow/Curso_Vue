<template>
<div>
  <primeiro-componente/>
  <p>A linguagem que eu uso é: {{ Testando }}</p>
</div>
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue'
    export default{
      name:'app',
      components: {
        PrimeiroComponente 
      },
      data() {
        return {
          Testando:"Vue.js"
        }
      },
    }
</script>
