<template>
    <div class="les-tables">
        <br>
        <input type="radio" v-model="n">10
        <input type="radio" v-model="n">13
        <TableMultiplication v-for="tables in 10" v-bind:n="parseInt(tables)"/>
        <hr/>
    </div>
</template>

<script>
    import TableMultiplication from '../components/TableMultiplication.vue'

    export default {
        name: 'tables',
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
    .les-tables {
        display: block;
    }
</style>