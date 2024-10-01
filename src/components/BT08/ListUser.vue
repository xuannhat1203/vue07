<template>
  <div>
    <button @click="handleClick">Add User</button>
    <FormAddUser :value="data"></FormAddUser>
  </div>
</template>

<script setup>
import { ref } from 'vue';
import FormAddUser from './FormAddUser.vue';

const data = ref(false);

const handleClick = () => {
  data.value = true;
};

</script>
