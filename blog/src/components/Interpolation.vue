<template>


    <h1>Name :{{name}}</h1>
    <h2>Address:{{address}}</h2>
    <h3>Age:{{age}}</h3>
    <h3>CheckNumber:{{checkNumber==99}}</h3>
    <h4>CallBack :{{getName()}}</h4>


<span>{{setData("Azil Hossain")}}</span>

    <p>{{getData()}}</p>

</template>

<script>
    export default {
        name: "Interpolation",
        data() {
            return {
                name: "Irfan",
                email:"irfanhossain701@gmail.com",
                address: "Oli Mia Hat",
                age: "30",
                checkNumber:8899,
                getName: function () {
                    return "Callback Function"
                }
            }
        },
        methods:{
            setData(name){
                return name;
            },
            getData(){
                return {
                    Book:"Bangla English",
                    Author:"JACKSON",
                    Email:this.email

                }
            }

        }
    }
</script>


<style scoped>

</style>