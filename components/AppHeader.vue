<template>
    <div class="header container-fluid">
        <h1 class="title">Jokes</h1>
        <ul>
            <li><nuxt-link to="/">Home</nuxt-link></li>
            <li><nuxt-link to="/jokes">Jokes</nuxt-link></li>
            <li><nuxt-link to="/about">About</nuxt-link></li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'Header'

}
</script>

<style>
    .header{
        
        width: 100%;
        background: lightgray;
        display: flex;
        justify-content: space-between;
        margin-bottom: 1rem;
        padding-bottom: 1rem;
        border-bottom: 1px dotted #ccc
    }
    /* .header ul li{
        float:right;  
    } */

    .header ul{
        display: flex;
        text-decoration: none;
        list-style: none;
        
    }
    .header a{
        display: inline-block;
        margin-right: 0.5rem;
        /* text-decoration: none; */
        color:black;
        padding: 0.3rem 1rem;
    }

</style>
