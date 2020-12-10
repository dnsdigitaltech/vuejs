<template>
  <div class="container mt-3 box">
    <div class="row">
      <div class="col-12 p-4">
        <p>Mecanismo para alterar o valor do nome</p>
        <button @click="alterarnome">Alterar nome</button>
        <app-detalhe :meunome="onomeoriginal"></app-detalhe>
      </div>
    </div>

  </div>
</template>

<script>
  import Detalhe from './components/Detalhe.vue'
  export default{
    components: {
      'app-detalhe': Detalhe
    },
    data() {
        return {
            onomeoriginal: "Davi"
        }
    },
    methods: {
      alterarnome(){
        this.onomeoriginal = "Carlos"
      }
    },
  }
</script>

<style scoped>
  .box{
    border: 2px solid black;
    background-color: rgb(200, 200, 200);
  }
</style>