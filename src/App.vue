<template>
<div>
  <primeiro-componente/>
  <p>A linguagem que eu uso é: {{ Testando }}</p>
  <life-cycle />
  <pessoa />
</div>
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/Pessoa.vue'

    export default{
      name:'app',
      components: {
        PrimeiroComponente,
        LifeCycle,
        Pessoa
      },
      data() {
        return {
          Testando:"Vue.js"
        }
      },
    }
</script>
