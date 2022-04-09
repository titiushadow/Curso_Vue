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

<!-- usando @click para mostrar o E-mail -->
  <div>
    <button @click="showEmail">
    {{ textoBotao }}
    </button>
  </div>

  <!-- v-show -->
  <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>

  <p>Para acessar meu portifólio
    <a v-bind:href="meu_link">
      basta clicar aqui!
    </a>
  </p>
  <Picture />

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
      email: 'mesaque1212@gmail.com',
      meu_link: "https://github.com/titiushadow",
      textoBotao: 'Mostrar e-mail'
    }
  },

  // Metodo para mostrar e esconder E-mail
  methods: {
    showEmail(){
      this.mostrar_email = !this.mostrar_email
      if(!this.mostrar_email) {
        this.textoBotao = 'mostrar e-mail'
      } else {
          this.textoBotao = 'Esconder e-mail'
      }
    }
  },
}
</script>