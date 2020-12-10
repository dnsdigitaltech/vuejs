<template>
  <div>
    <p>Esta é a App.vue</p>
    <app-servidor></app-servidor>
    
  </div>
</template>

<script>

import Servidor from './components/Servidor';
export default{
  components: {
    'app-servidor': Servidor
  }
}
</script>

<style>

</style>
