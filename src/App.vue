<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <!-- <Data /> -->
  <TemplateVue />
</template>

<script>
// import Data from "./components/parent-to-child/Data.vue"
import TemplateVue from './components/template/Template.vue';
export default {
  name: 'App',
  components: {
    // Data
    TemplateVue
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
