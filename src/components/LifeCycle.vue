<template>
    <h1>My name is: {{ nome }}</h1>    
</template>

<script>
export default {
    name:'LifeCycle',
    data() {
        return {
            nome: 'Mesaque'
        }
    },
    created(){
        setTimeout(() => {
            this.nome = 'Meseikers'
        }, 1000);  
    },
    mounted() {
        setTimeout(() => {
            this.nome = 'João'
        }, 2000);
    },
}
</script>