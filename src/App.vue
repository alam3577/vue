<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <!-- <Data /> -->
  <!-- <TemplateVue /> -->
  <!-- <Styles /> -->
  <!-- <Computed /> -->
  <Watcher />
</template>

<script>
// import Data from "./components/parent-to-child/Data.vue"
// import TemplateVue from "./components/template/Template.vue";
// import Styles from "./components/class-style-binding/Styles"
// import Computed from './components/computed/Computed.vue';
import Watcher from './components/watchers/Watcher.vue';

export default {
  name: 'App',
  components: {
    // Data
    // TemplateVue
    // Styles
    // Computed
    Watcher
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
