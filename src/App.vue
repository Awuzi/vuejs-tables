<template>
    <div id="app">
        <nav class="topnav">
            <router-link class="texte" to="/">&nbsp;Home</router-link>
            <router-link class="texte" to="/tables">&nbsp;Les tables</router-link>
        </nav>
        <img alt="Vue logo" src="./assets/logo.png" width="100" height="100">
        <router-view/>
    </div>
</template>

<script>
    export default {
        name: 'app'
    }
</script>

<style>
    html {
        padding: 0;
        margin: 0;
    }

    .topnav {
        text-align: center;
        padding-bottom: 10px;
        background-color: darkblue;
        padding-top: 10px;
    }

    .texte {
        color: white;
        margin-left: 10px;
        margin-right: 20px;
        text-decoration: unset;
    }

</style>
