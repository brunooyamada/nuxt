<template>
    <div>
        <div v-for="product in products" :key="product.id"
        class="border-b border-gray-400 py-3"
        >
            {{ product.title }}
        </div>
        
        <h1 class="text-lg font-bold">Produtos</h1>
        <NuxtLink to="/produtos/produto-a">Produto A</NuxtLink>
        <NuxtLink to="/produtos/produto-b">Produto B</NuxtLink>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam tempus diam vitae ante tincidunt, et blandit tellus pharetra. Suspendisse lobortis enim in orci egestas consectetur. Pellentesque a hendrerit nulla. Sed pulvinar nunc diam, ut blandit diam tristique vel. Suspendisse eu aliquet justo. In malesuada odio quis fermentum varius. Vestibulum tempus, sem eget consequat commodo, ex magna consequat dui, et ultrices libero erat ac dui. </p>
    </div>
</template>

<script>

export default ({
    name: "",

    data() {
        return {
        };
    },

    async asyncData({ $axios }) {
        
        const products = await $axios.$get('https://jsonplaceholder.typicode.com/posts?_limit=3');
        return {
            products,
        };
    },
    
    methods: {},
})
</script>
