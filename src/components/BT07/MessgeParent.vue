<template>
    <MessgeChildren @buttonAlert="handleAlert" />
</template>

<script setup>
    import MessgeChildren from './MessgeChildren.vue';
    function handleAlert(msg){
        alert(msg)
    }
</script>

<style>

</style>