<template>
    <div>
        <h4>Count: {{ count }}</h4>
        <CountChildren @handleRaise="handleClick"></CountChildren>
    </div>
</template>

<script setup>
import { ref } from 'vue';
import CountChildren from './CountChildren.vue';

const count = ref(0); 

function handleClick(msg) {
    count.value = msg; 
}
</script>

<style>
</style>
