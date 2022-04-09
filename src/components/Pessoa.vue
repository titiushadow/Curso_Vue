<template>
<div>
  <h2>Esta é a descrição da pessoa: {{ name }}</h2>
  <info :email="email" :esta_codando=true />
  <Form />
</div>
</template>

<script>
  import info from './info.vue'
  import Form from './Form.vue'

export default {
  name: 'Pessoa',
  components: {
    info,
    Form
  },
  data() {
    return {
      name: 'Mesaque',
      email: 'mesaque1212@gmail.com'
    }
  },
}
</script>