<template>
    <h1>Child Component</h1>
    <p>{{name}}</p>
    <p>{{user.name }} AND {{user.email}}</p>
    <button v-on:click="getData()">CLICK ME</button>
</template>

<script>
    export default {
        name: "Child",
        props:{
            name:String,
            user:Object,
            getData:Function
        }
    }
</script>

<style scoped>

</style>