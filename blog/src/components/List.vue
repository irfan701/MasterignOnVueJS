<template>


    <h2>List</h2>
    <table>

        <tr v-for="item in technology" :key="item">
            <td>
                {{item}}
            </td>

        </tr>
    </table>


    <br><br>

    <table>

        <tr v-for="item in user" :key="item">
            <td>
                {{item.name}}

            </td>
            <td>{{item.age}}</td>

        </tr>
    </table>
</template>

<script>
    export default {
        name: "List",
        data() {
            return {
                technology: ['PHP', 'JAVASCRIPT', 'NODE JS', 'EXPRESS JS'],
                user: [
                    {name: "Irfan", age: 21},
                    {name: "Hossain", age: 31},
                    {name: "Arman", age: 41}

                ]
            }
        }
    }
</script>

<style scoped>

</style>