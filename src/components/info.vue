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
</template>
<script>
export default {
  name: 'Info',
  data() {
    return { 
      esta_codando: false,
      mostrar_email: true,
      email: 'mesaque1212@gmail.com'
    }
  }
}
</script>