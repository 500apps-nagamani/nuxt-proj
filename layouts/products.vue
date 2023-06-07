<template>
    <div>
        <header class="m-4">
            
                
                <ul class="flex gap-4">
                                    
                    <li>
                        <NuxtLink to="/">Home</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/about">About</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/products">Products</NuxtLink>
                    </li>
                </ul>
            
        </header>
        <div>
            <slot />
        </div>
       
    </div>
    
</template>



<style scoped>
.router-link-exact-active{
        color: aquamarine;
    }
    nav {
        background-color: aquamarine;
    }
</style>