<template>
    <div>
        <button @click="ativar">Cliquei aqui!</button>
        <span v-show="ativou">Ativado!</span>
    </div>
</template>

<script>
export default {
    nome: 'Reutilizacao',
    data() {
        return {
            ativou: false           
        }
    },
    
    // Metodo para ativar o botão 
    methods: {
        ativar() {
            this.ativou = !this.ativou
        }
    },
}
</script>