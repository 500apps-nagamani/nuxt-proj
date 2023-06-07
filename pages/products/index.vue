
<template>
    <div>
    
        
        <div class="grid grid-cols-4 gap-4 mt-5">
            <div v-for="p in products">
               <ProductCard :product="p"/>
            </div>
        </div>
       
    </div>
</template>

<script setup >
const { data : products } = await useFetch("https://fakestoreapi.com/products");
definePageMeta({
        layout:'products'
    })
useHead({
    title : "Nuxt Dojo | Products",
    meta : [{name:"description",content:"About Products"}]
})
   
</script>


<style scoped>
    

</style>