<template>
    <div>
        <h4>Id to delete: {{ id }}</h4>
        <TodoItem @DeleteItem="handleDelete"></TodoItem>
    </div>
</template>

<script setup>
import { ref } from 'vue';
import TodoItem from './TodoItem.vue';

const id = ref(0); 

function handleDelete(msg) {
    id.value = msg; 
}
</script>

<style>
</style>
