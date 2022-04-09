<template>
<h2>Meu primeiro form com VUE</h2>

<form action="" @submit="enviarformulario($event)">
    <div>
        <input type="text" v-model="name">        
    </div>

     <div>
        <input type="text" v-model="email">
    </div>

     <div>
        <submit />
    </div>
</form>
</template>

<script>
import InputText from './Form/InputText.vue'
import Submit from './Form/Submit.vue'
export default {
    name: 'Form',
    components: {
        InputText,
        Submit
    },
    data() {
        return {
            name: "",
            email: ""            
        }
    },
    methods: {
        enviarformulario(e){

            e.preventDefault();

            const nome = this.name;
            const email = this.email;
            
            console.log('Formulario enviado');
            console.log('O nome é:' + nome);
            console.log('O email é:' + email);

            // Ajax



            // Inserir no banco os dados

            
        }
    },
}
</script>
   