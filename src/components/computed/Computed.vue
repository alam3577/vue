<template>
    <!-- Recalculating occur In template -->

    <!-- <div>Hello {{ (dollar * rupees) / discount }}</div>
    <div>Hello {{ (dollar * rupees) / discount }}</div>
    <div>Hello {{ (dollar * rupees) / discount }}</div> -->

    <!-- Recalculating occur In Method -->

    <!-- <div>Hello {{ calculateDiscountMethod() }}</div>
    <div>Hello {{ calculateDiscountMethod() }}</div> -->

    <!-- Computed is cache based So, recalculating will not occur -->
    <div>Hello {{ calculateDiscount }}</div>
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name:"Computed",
    data(){
        return {
            dollar: 1000,
            rupees: 2000,
            discount: 10,
        }
    },
    methods: {
        calculateDiscountMethod() {
            return (this.dollar * this.rupees) / this.discount
        }
    },
    computed: {
        calculateDiscount() {
            return (this.dollar * this.rupees) / this.discount
        } 
    }
}
</script>