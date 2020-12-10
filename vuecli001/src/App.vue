<template>
  <div>
    <p>App.vue</p>
    <app-servidors></app-servidors>
    <app-servidor></app-servidor>
    <servidor></servidor>
  </div>
</template>

<script>

import Servidor from './components/servidor/Servidor';
export default{
  components: {
    'app-servidors': Servidor,
    'appServidor': Servidor,
    Servidor
  }
}
</script>

<style>

</style>