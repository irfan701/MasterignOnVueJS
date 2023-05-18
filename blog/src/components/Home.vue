<template>
    <h1>Hello World</h1>
    <Teacher name="IRFAN HOSSAIN"/>
    <Student :name="name"/>

</template>


<script>
    import Teacher from "./Teacher.vue";
    import Student from "./Student.vue";
    export default {
        name: "Home",
        data() {
            return {
                name: "Irfan"
            }
        },
        components: {
            Teacher,
            Student
        },


    }

</script>


<style scoped>
    h1 {
        color: red;
    }
</style>