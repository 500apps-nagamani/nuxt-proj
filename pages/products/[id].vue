
<template>
    <div class="p-5">
        <Head>
            <Title>Nuxt Dojo | {{ product.title }}</Title>
            <Meta name="description" :content="product.description"/>
        </Head>
        <div class="mt-4">
           <ProductDetails :product="product"/>
        </div>
    </div>
</template>


<script setup >

definePageMeta({
        layout:'products'
    })
    const { id } = useRoute().params
    
    const uri = "https://fakestoreapi.com/products/" + id

    const {data : product} = await useFetch(uri,{key:id})


    if (!product.value) {
        throw createError({statusCode:404, statusMessage:"Product not found"})
    }
</script>


<style scoped>

</style>