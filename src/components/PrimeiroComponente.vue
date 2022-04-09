<template>
    <div>
        <h1>Olá vue</h1>
        <p>Meu nome é: {{ nome }}, E meu trabalho é: {{ Profissão }}</p>
    </div>
</template>

<script>
export default {
    name: 'PrimeiroComponente',
    data() {
        return {
            nome: "Mesaque",
            Profissão: "Programador"
        }
    },
}
</script>