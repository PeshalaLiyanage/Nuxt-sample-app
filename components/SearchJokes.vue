<template>
    <div class="search container-fluid">
        <div class="form-one">
            <form class="form-group" @submit.prevent="onSubmit">
            <input type="text" v-model="text"  placeholder="Search jokes...">
            <input type="submit" value="Search" class="btn">
        </form>
        </div>
        

    </div>
</template>

<script>
export default {
    name:'SearchJokes',
    data(){
        return{
            text:''
        }
    },
    methods:{
        onSubmit(){
            this.$emit("search-text",this.text);
            this.text="";

        }
    }

}
</script>

<style>
    .btn{
        background:lightgrey;
    }
    .search{
        width: 70%; 
        margin-left: auto;
        margin-right: auto;
       

    }
    input[type="text"]{
        width: 60%;
        /* margin-left: auto;
        margin-right: auto; */
    }
    .form-one{
        margin-left: auto;
        margin-right: auto;
        width: 100%;
    }
   
</style>
