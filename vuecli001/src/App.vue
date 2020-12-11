<template>
  <div class="container mt-3 box">
    <p>(App.vue) Nome = {{nome}}</p>
    <button @click="alterar">Alterar</button>
    <hr>
    <app-componente :meunome="nome" @nomeAlterado="nome = $event"></app-componente>
  </div>
</template>

<script>
  import componente from './components/componente'
  export default{
    components: {
      'app-componente': componente
    },
    data() {
      return {
        nome: "Davi"
      }
    },
    methods: {
      alterar(){
        this.nome = 'Nathan'
      }
    },
  }
</script>
