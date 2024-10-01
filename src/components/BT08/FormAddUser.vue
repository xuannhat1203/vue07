<template>
  <div v-if="value" class="form-container">
    <h2>Form Add User</h2>
    <form @submit.prevent="submitForm">
      <div class="form-group">
        <label for="name">Name</label>
        <input type="text" id="name" v-model="name" required />
      </div>
      <div class="form-group">
        <label for="email">Email</label>
        <input type="email" id="email" v-model="email" required />
      </div>
      <div class="form-group">
        <label for="address">Address</label>
        <input type="text" id="address" v-model="address" required />
      </div>
      <button type="button" @click="closeForm" class="close-btn">Close</button>
    </form>
  </div>
</template>

<script setup>
const props = defineProps({
  value: Boolean,
});
</script>

<style></style>
