<template>
  <header>
    <h1>ESTE É O HEADER</h1>
    <p>Treinando com um componente Vue em AEM</p>
    <p> {{ text }} </p>
    <p> {{ checkbox ? 'isChecked' : 'inNotChecked' }} </p>
  </header>
</template>

<script>
// Imports

export default {
  name: 'CustomHeader',
  props: {
    text: {
      type: String,
      default: 'Texto padrão'
    },
    checkbox: {
      type: Boolean,
      default: false
    }
  }
}
</script>

<style>
header {
  background-color: #ddd;
  padding: 20px;
}
h1 {
  color: red;
}
</style>
