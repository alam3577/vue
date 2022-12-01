<template>
  <div>
    <h1 v-if="show">Hi, I am from {{name}} Component</h1>
    <h1 v-else>Hi this is else Condition, I am from {{name}} Component</h1>
    <button v-on:click="consoleClickHandler()">Click to console</button>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'Home',
  props: {
    name: String
  },
  data(){
     {
        return {show: true}
     }
  },
  methods:{
    consoleClickHandler(){
        this.show = !this.show
    }
  }
}
</script>