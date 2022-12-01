<template>
    <div>
        <h1>Welcome to Styling of vue js</h1>
        <!-- Style with classes -->
        <h3 class="paragaraph">Styling this content with Class name</h3>
        <!-- Inline Styling -->
        <h3 v-bind:style="{color: 'red'}">This content belongs to inline styling</h3>
        <!-- Styling with Object -->
        <h3 v-bind:class="{display:show}">This content belongs to Object styling</h3>
        <button v-on:click="changeBackgroundColor">Click Me to change Color</button>
    </div>
</template>

<script>
export default {
   // eslint-disable-next-line vue/multi-word-component-names
   name: "Styles",
   data(){
      return {
        show: true
      }
   },
   methods: {
    changeBackgroundColor(){
      this.show = !this.show
    }
   }
}
</script>

<style scoped>
  .paragaraph {
       color: green;
  }
  .display {
    color: darkgoldenrod;
  }
</style>