<template>
    <h4>Children Component: {{ propName }} </h4>
</template>

<script setup>
    const props = defineProps({
        propName:String,
    })
</script>

<style>

</style>