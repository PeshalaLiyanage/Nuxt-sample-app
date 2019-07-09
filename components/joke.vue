<template>
    <div class="joke">
        <nuxt-link :to="'jokes/'+id" >
             {{joke}}
        </nuxt-link>
        
    </div>
</template>

<script>
export default {
    name: "Joke",
    props:["joke", "id"]
}
</script>

<style>
    .joke{
        width: 80%;
        margin-left: auto;
        margin-right: auto;
        background: lightgray;
        padding:0.5rem;
        /* border-bottom: 1px dotted black; */
        margin-bottom: 0.5em;
       font-family: cursive;
        
        
    }
    .joke a{
        color: #000;
        text-decoration: none;
        
    }

</style>
