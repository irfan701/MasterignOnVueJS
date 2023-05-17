<template>
    <h1>Email:{{email}}</h1>
    <br>
    <h1>Password:{{password}}</h1>

    <input type="text" placeholder="Email" v-model="email">
    <br>
    <input type="text" placeholder="Password" v-model="password">
    <br>
    <button v-on:click="getData()">Get Value</button>

    <p>Get Checkbox & Radio Button Values</p>
    <h3>Technology</h3>

    <label for="java">java</label>
    <input type="checkbox" value="java" id="java" v-model="technology">

    <label for="php">php</label>
    <input type="checkbox" value="php" id="php" v-model="technology">

    <label for="express">Express</label>
    <input type="checkbox" value="express" id="express" v-model="technology">

    <br>
    <p>{{technology}}</p>

    <br><br>

    <h3>Who I am</h3>
    <label for="student"></label>
    <input type="radio" value="student" name="who" id="student" v-model="who">

    <label for="developer"></label>
    <input type="radio" value="developer" name="who" id="developer" v-model="who">


    <br>
    <p>I am :{{who}}</p>

    <br><br>
</template>

<script>
    export default {
        name: "TwoWayBinding",
        data(){
            return{
                email: null,
                password:null,
                technology:[],
                who:null
            }
        },
        methods:{
            getData() {
                console.warn("HEY"+ this.email+' '+this.password)
            }
        }
    }
</script>

<style scoped>

</style>