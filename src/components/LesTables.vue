<template>
    <div>
        <span v-for="k in choice" :key="k">
      <p>
        <table-multiplication v-bind:n="parseInt(k)"/>&nbsp;
      </p>
    </span>
    </div>
</template>

<script>
    import TableMultiplication from './TableMultiplication.vue'

    export default {
        name: 'LesTables',
        components: {
            TableMultiplication
        },
        props: {
            n: Number,
            choice: Number
        }
    }
</script>

<style>
    p {
        display: inline-block;
        margin: 0px 20px;
    }
</style>