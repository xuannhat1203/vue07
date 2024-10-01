<template>
    <button @click="handleDelete">Delete</button>
</template>

<script setup>
    const emit = defineEmits(["DeleteItem"]);
    function handleDelete(){
        emit("DeleteItem",1)
    }
</script>

<style>

</style>