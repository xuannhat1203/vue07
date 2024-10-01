<template>
    <div>
        <p>ID: {{ obj.id }}</p>
        <p>Product Name: {{ obj.name }}</p> 
        <p>Quantity: {{ obj.quantity }}</p>
        <p>Price: {{ obj.price }}</p>
    </div>
</template>

<script setup>
    const props = defineProps({
        obj: Object, 
    })
</script>

<style>
</style>
