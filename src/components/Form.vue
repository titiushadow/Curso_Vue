<template>
<h2>Meu primeiro form com VUE</h2>
    <div>
        <input-text />
    </div>

     <div>
        <input-text />
    </div>

     <div>
        <submit />
    </div>
</template>

<script>
import InputText from './Form/InputText.vue'
import Submit from './Form/Submit.vue'
export default {
    name: 'Form',
    components: {
        InputText,
        Submit
    }

}
</script>
   