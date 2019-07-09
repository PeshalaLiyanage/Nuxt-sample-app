<template>
    <div  class="joke">
        <p>{{joke}}</p>
        <hr>
        <nuxt-link to="/jokes">Back to jokes</nuxt-link>
    </div>
    
    
</template>

<script>
import axios from 'axios';
export default {
    data(){
        return {
            joke: {}
        }
    },
    async created(){
        const config = {
            headers:{
                Accept: "application/json"
            }
        };
        try {
            const res = await axios.get(`https://icanhazdadjoke.com/j/${this.$route.params.id}`,config);
            console.log(res.data.joke);
            this.joke = res.data.joke;
        } catch (err) {
            console.log(err);
        }
    },
     head(){
        return{
            title: this.joke,
            meta:[
                {
                    hid: "description",
                    name: "description",
                    content: "The best place for jokes"
                }
            ]
        };
    }


}
</script>

<style>

</style>
