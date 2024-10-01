<template>
    <Accordion>
      <template #header="{ item }">
        <span>Tiêu đề Accordion {{ item.id }}</span>
      </template>
      <template #content="{ item }">
        <p>{{ item.title }}</p>
        <p>Thêm nội dung tùy chỉnh ở đây cho Accordion {{ item.id }}</p>
      </template>
    </Accordion>
  </template>
  
  <script setup>
  import Accordion from './Accordion.vue';
  </script>
  