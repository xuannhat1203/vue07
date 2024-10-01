<template>
    <button @click="handleClick">Raise</button>
</template>

<script setup>
import { ref } from 'vue';

const emit = defineEmits(["handleRaise"]);
const count = ref(0); 
function handleClick() {
    count.value++;
    emit("handleRaise", count.value); 
}
</script>

<style>
</style>
