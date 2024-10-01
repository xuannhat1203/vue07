<template>
    <button @click="handleClick">Handle Alert</button>
</template>

<script setup>
    const emit = defineEmits(["buttonAlert"]);
    function handleClick(){
        emit("buttonAlert","Welcome to Rikkei Education")
    }
</script>

<style>

</style>