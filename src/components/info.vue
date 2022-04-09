<template>
<!-- v-if and v-else -->
  <p v-if="esta_codando">Estou codando no momento.</p>
  <p v-else>Estou em busca de novas oportunidades</p>

<!-- Lista usando (v-for) -->
  <p>Utilizo as seguintes tecnologias para back-end:</p>
  <ul>
    <li v-for="(technology,index) in backend_technologies" v-bind:key="index">{{ technology }}</li>
  </ul>
  <p>Utilizo as seguintes tecnologias para fronend:</p>
    <ul>
      <li v-for="technology in frontend_technologies" :key="technology.id">
        {{ technology.language }}
      </li>
      
    </ul>

<!-- usando @click para mostrar o E-mail -->
  <div>
    <button @click="showEmail">
    {{ textoBotao }}
    </button>
  </div>

  <!-- v-show -->
  <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>

<!-- link para o portifólio -->
  <p class="teste">Para acessar meu portifólio
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
      textoBotao: 'Mostrar e-mail',

      //Array para renderização de listas (v-for)
      backend_technologies: ['PHP/Laravel', 'JavaScript', 'PHP', 'Python'],

      // Array de objetos com (v-for)
      frontend_technologies: [
        {id: 1, language: 'HTML'},
        {id: 2, language: 'CSS'},
        {id: 3, language: 'Vue'}       
      ]
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

<style>
  .paragrafo-pai {
    color:red;
  }

</style>