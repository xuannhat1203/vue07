<template>
    <ProductChildren :obj="object"></ProductChildren>
</template>

<script setup>
    import ProductChildren from './ProductChildren.vue';
    
    const object = {
        id: 1,
        name: "Iphone 16 promax",
        quantity: 10,
        price: 3000,
    }
</script>

<style>
</style>
