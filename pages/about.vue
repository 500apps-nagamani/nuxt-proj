




<template>
    <div class="shadow-l bg-primary">
    
        <h1>About page</h1>
        <p>Welcome to About page</p>
        <button>Continue</button>
        <p>{{ data }}</p>
    </div>
</template>



<script setup >
   const {data} =await useFetch("/servers/api/index")
</script>


<style scoped>
    button{
        background-color: aqua;
        width: 70px;
        height: 40px;
        margin: 5px;
        border-radius: 8px;
        border-color:  black;
        border-width: 1px;
        font-size: 12px;
    }
</style>