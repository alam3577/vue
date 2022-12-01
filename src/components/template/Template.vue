<template>
    <div>
        <p v-html="htmlTemplate"></p>
        {{(a+b)}}
        <h3>Count {{count}} {{(count%2===0? "Even": "Odd")}}</h3>
        <button v-bind:disabled="diabledBtn" v-on:click="IncCounter">Click</button>
    </div>
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: "Template",
    data(){
        return {
            htmlTemplate: "<h1> Welcome to the Template Pages </h1>",
            a: 30,
            b: 70,
            count: 0,
            diabledBtn: true
        }
    },
    
    methods: {
        IncCounter(){
           this.count = this.count + 1;
        }
    }
}
</script>