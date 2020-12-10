<template>
  <div class="container mt-3 box">
    <button @click="executar(0)" class="btn btn-primary m-1">Click 0</button>
    <button @click="executar(100)" class="btn btn-primary m-1">Click 100</button>
    <button @click="executar(200)" class="btn btn-primary m-1">Click 200</button>
    <app-componente :meuvalor="valor"></app-componente>
  </div>
</template>

<script>
  import componente from  './components/componente';
  export default{
    components:{
        'app-componente': componente
    },
    data() {
      return {
        valor: 0
      }
    },
    methods: {
      executar(value){
        this.valor = value
      }
    },
  }
</script>
