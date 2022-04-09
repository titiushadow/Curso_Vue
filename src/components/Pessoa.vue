<template>
<div>
  <h2>Esta é a descrição da pessoa: {{ name }}</h2>
  <info />
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
      name: 'Mesaque'
    }
  },
}
</script>