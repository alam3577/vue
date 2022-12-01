<template>
    <div>
        <h1>Welcome to the data page</h1>
        <DataChild :users="users"/>  
    </div>
</template>

<script>
import DataChild from "./DataChild.vue";
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: "Data",
    data () {
        return {
           users: [
            {id: "123", name: "sajjad alam", email: "sajjad@gmail.com"},
            {id: "124", name: "Sabbaj", email: "sabbaj@gmail.com"},
            {id: "125", name: "sibani", email: "siani@gmail.com"},
            {id: "126", name: "pritam", email: "pritam@gmail.com"},
            {id: "127", name: "ananya", email: "ananya@gmail.com"},
            {id: "128", name: "najrul", email: "najrul@gmail.com"},
           ]
        }
    },
    components: {
        DataChild
    }
}
</script>

<style scoped>
  div{
    padding: 3rem;
  }
  table{
    border: 1px solid black;
  }

  td{
    border: 1px solid black;
  }
</style>