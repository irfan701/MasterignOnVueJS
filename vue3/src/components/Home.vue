<template>
    <h1>Pass Data To Child Component</h1>
    <br>
    <Child name="Irfan Hossain" :user="user" :getData="getData"/>
</template>

<script>
    import Child from "./Child.vue";
    export default {
        name: "Home",
        components:{
            Child
        },data(){
            return{
                user:{name:"Hasan",email: "hasan@gmail.com"}
            }
        },
        methods:{
            getData() {
                alert("Parent Function Call")
            }
        }
    }
</script>

<style scoped>

</style>