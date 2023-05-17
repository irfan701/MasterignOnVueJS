<template>
    <h1>If Else Condition</h1>

    <h3 v-if="show">If Condition</h3>
    <h3 v-else>Else Condition</h3>

    <button v-on:click="show=!show">Toggle Switch</button>
</template>

<script>
    export default {
        name: "Conditional",
        data() {
            return {
                show:true
            }
        }
    }
</script>

<style scoped>

</style>