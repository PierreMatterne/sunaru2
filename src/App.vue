<template>
  <compas :direction="direction" />
  <window />
  <main-input />
  <inventory /> 
</template>

<script>
  import Compas from './components/Compas.vue';
  import Inventory from './components/Inventory.vue';
  import MainInput from './components/MainInput.vue';
  import Window from './components/Window.vue';

  export default {
    name: 'App',
    data(){
      return {
        direction: 'N',
      }
    },
    components: {
      Compas,
      Inventory,
      MainInput,
      Window,
    }
  }
</script>

<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>
