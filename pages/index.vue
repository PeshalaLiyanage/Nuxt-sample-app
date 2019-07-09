<template>
  <div class="container welcome">
    <h1> Welcome to the best corny jokes</h1>
  </div>
</template>

<script>


export default {
   head(){
        return{
            title: 'Welcome',
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
.welcome{
  text-align: center;
}

</style>
