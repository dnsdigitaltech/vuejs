<template>
  <div>
    <p>App.vue</p>
    <comp1/>
    <comp2/>
  </div>
</template>

<script>
  import comp1 from './components/comp1';
  import comp2 from './components/comp2';
  export default{
    components: {
      comp1,
      comp2
    }
  }
</script>

<style>

</style>