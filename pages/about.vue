<template>
    <div class="about container">
        <h1>This is the about page</h1>
    </div>
</template>

<script>
export default {    
    head(){
        return{
            title: 'About the app',
            meta:[
                {
                    hid: "description",
                    name: "description",
                    content: "The best place for jokes"
                }
            ]
        };
    }

};
</script>

<style>
.about{
    text-align: center;
}

</style>
