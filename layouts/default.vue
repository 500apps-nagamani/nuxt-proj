<template>
    <div>
        <header class="m-4">
            <nav class="shadow-sm bg-blue flex justify-between p-4">
                
                <ul class="flex gap-4">
                    <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ84sLyP5PQYsoGKdnhRCwt3DJeSmFvHOdmMA&usqp=CAU" />                    
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
            </nav>
        </header>
        <div class="container mx-4 p-4">
        <slot />
    </div>
  
    </div>
    
    
</template>

<style scoped>
    .router-link-exact-active{
        color: aquamarine;
    }
    img{
        height: 50px;
        width:50px;
    }
  </style>