

<template>
    <div>
        <div class="card text-center">
            <img :src="product.image" alt="thumb" />
            <p class="font-bold m-4 text-center">{{ product.title }}</p>
            <NuxtLink :to="`/products/${product.id}`">
            <p class="btn">View Details</p>
        </NuxtLink>
         </div>
    </div>
</template>

<script setup>
    const {product} = defineProps(['product'])
</script>

<style scoped>
img{
    height:60px;
    width:50px;
    margin: 0 auto;
    }
    
</style>