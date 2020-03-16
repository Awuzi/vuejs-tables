<template>
    <div>
        <br>
        <label for="user-input"> Entrez une valeur : </label>
        <input id="user-input" type="text" v-model="n">
        <div v-if="!isNaN(n)">
            <TableMultiplication v-bind:n="parseInt(n)"/>
        </div>
    </div>
</template>

<script>
    import TableMultiplication from '../components/TableMultiplication.vue'

    export default {
        name: 'home',
        data: function () {
            return {
                n: 0
            }
        },
        components: {
            TableMultiplication,
        }
    }
</script>

<style>
    html body {
        font-family: "Avenir", Helvetica, Arial, sans-serif;
        text-align: center;
        padding: 0;
        margin: 0;
    }

</style>
