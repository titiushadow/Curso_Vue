<template>
<div>
  <Header :esta_logado="true" />
  <primeiro-componente/>
  <p class="paragrafo-pai">A linguagem que eu uso é: {{ Testando }}</p>
  <life-cycle />
  <pessoa />
</div>
</template>

<script>
import Header from './components/Header.vue' 
import PrimeiroComponente from './components/PrimeiroComponente.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/Pessoa.vue'

    export default{
      name:'app',
      components: {
        Header,
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

<style>
  body {
    background-color: #333;
    color: #fff;
  }

  a {
    color:#ff0000;
  }

  .teste {
    background-color: #000;
  }
</style>
