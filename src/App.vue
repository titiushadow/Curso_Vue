<template>
<div>
  <primeiro-componente/>
  <p>A linguagem que eu uso é: {{ Testando }}</p>
  <life-cycle />
</div>
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue'

    export default{
      name:'app',
      components: {
        PrimeiroComponente,
        LifeCycle
      },
      data() {
        return {
          Testando:"Vue.js"
        }
      },
    }
</script>
