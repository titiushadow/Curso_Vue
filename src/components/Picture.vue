<template>
  <img :src="avatar" :alt="descricao">
  <MudarImagem @mudar-imagem="mudarImagem" />
</template>
<script>
import MudarImagem from './MudarImagem.vue'
export default {
  components: { MudarImagem },
  name: 'Picture',
  data() {
    return { 
      avatar: "/img/avatar.png",
      descricao: "Mesaque"
    }
  },

//metodo para mudar de imagem
  methods: {
    mudarImagem() {
      this.avatar = "/img/avatar2.png"
    }
  }
}
</script>