<template>
<!-- v-if and v-else -->
  <p v-if="esta_codando">Estou codando no momento.</p>
  <p v-else>Estou em busca de novas oportunidades</p>
  <p>Utilizo as seguintes tecnologias:</p>
  <ul>
    <li>PHP/Laravel</li>
    <li>JavaScript</li>
    <li>PHP</li>
    <li>Python</li>
  </ul>

  <!-- v-show -->
  <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>

  <p>Para acessar meu portifólio
    <a v-bind:href="meu_link">
      basta clicar aqui!
    </a>
  </p>
  <picture />

</template>
<script>

import Picture from './Picture'
export default {
  name: 'Info',
  components: {
    Picture
  },
  data() {
    return { 
      esta_trabalhando: false,
      mostrar_email: false,
      url_portfolio: "https://github.com/titiushadow"
    }
  }
}
</script>