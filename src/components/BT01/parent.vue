<template>
    <children :propName="data"></children>
</template>

<script setup>
    import children from './children.vue';
    const data = "Rikkei Academy"
</script>

<style>

</style>