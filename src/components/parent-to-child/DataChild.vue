<template>
    <div>
    <h1>Welcome to the data child page</h1>
        <table>
            <thead><td>Id</td><td>name</td><td>email</td></thead>
            <tbody>
                <tr v-for="item in users" :key="item.id">
                    <td>{{item.id}}</td>
                    <td>{{item.name}}</td>
                    <td>{{item.email}}</td>
                </tr>
            </tbody>
        </table>
    </div>
</template>

<script>
export default {
    name: "DataChild",
    props: {
        users: Array
    }
}
</script>