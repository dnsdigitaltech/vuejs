<template>
  <div class="container mt-3 box">
    <p>Componente principal</p>
    <app-componente :valor1 = "nome"></app-componente>
  </div>
</template>

<script>
  import componente from './components/componente'
  export default{
    data() {
      return {
        nome: "Davi"
      }
    },
    components: {
      'app-componente': componente
    }
  }
</script>
