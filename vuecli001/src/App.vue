<template>
  <div class="container mt-3 box">
    <button @click="clickNome">Nome</button>
    <button @click="clickApelido">Apelido</button>
    <!--<p>{{nome}} {{apelido}}</p>-->
    <app-infopessoa 
    :infonome="nome" 
    :infoapelido="apelido">
    </app-infopessoa>
  </div>
</template>

<script>
import infopessoa from './components/infopessoa';

  export default{
    components:{
      'app-infopessoa':infopessoa
    },
    data() {
      return {
        nome: '',
        apelido: ''
      }
    },
    methods: {
      clickNome(){
        this.nome = 'Davi'
      },
      clickApelido(){
        this.apelido = 'Bernardo'
      }
    },
  }
</script>

<style scoped>

</style>