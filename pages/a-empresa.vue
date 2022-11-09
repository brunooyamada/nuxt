<template>
    <div>
        <div class="bg-gray-100">
            <div class="container mx-auto flex items-center space-x-4 h-10 mb-10">
                <NuxtLink :to="{ name: 'a-empresa' }">A empresa</NuxtLink>
                <NuxtLink to="/servicos">Serviços</NuxtLink>
            </div>
        </div>
        
        <div>
            <div class="container mx-auto">
                <h1 class="text-lg font-bold">A empresa</h1>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam tempus diam vitae ante tincidunt, et blandit tellus pharetra. Suspendisse lobortis enim in orci egestas consectetur. Pellentesque a hendrerit nulla. Sed pulvinar nunc diam, ut blandit diam tristique vel. Suspendisse eu aliquet justo. In malesuada odio quis fermentum varius. Vestibulum tempus, sem eget consequat commodo, ex magna consequat dui, et ultrices libero erat ac dui. </p>
            </div>
        </div>
    </div>
</template>

<script>

export default ({
    name: "",

    data() {
        return {
        };
    },
    
    methods: {},
})
</script>
