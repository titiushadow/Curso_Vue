<template>
    <div>
        <h1>Olá vue</h1>
        <p>Meu nome é: {{ nome }}, E meu trabalho é: {{ Profissão }}</p>
    </div>
    <MultiplosEventos />
    <Reutilizacao />
</template>

<script>

import Reutilizacao from './Reutilizacao.vue'
import MultiplosEventos from './MultiplosEventos.vue'
export default {
    name: 'PrimeiroComponente',
    components: {
        MultiplosEventos, 
        Reutilizacao      
    },
    data() {
        return {
            nome: "Mesaque",
            Profissão: "Programador"
        }
    },
}
</script>