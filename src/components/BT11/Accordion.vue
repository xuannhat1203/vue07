<template>
  <div class="accordion">
    <div
      v-for="obj in data"
      :key="obj.id"
      @click="handleClick(obj.id)"
      class="accordion-item"
    >
      <h4 class="accordion-header">
        <slot name="header" :item="obj">{{ `Accordion ${obj.id}` }}</slot>
      </h4>
      <div class="accordion-content" v-show="obj.status">
        <slot name="content" :item="obj">
          <p>{{ obj.title }}</p>
        </slot>
      </div>
    </div>
  </div>
</template>

<script setup>
import { reactive } from "vue";

const data = reactive([
  {
    id: 1,
    title:
      "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Amet maxime commodi doloremautem error, cumque facere similique aliquid adipisci a",
    status: false,
  },
  {
    id: 2,
    title:
      "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Amet maxime commodi doloremautem error, cumque facere similique aliquid adipisci a",
    status: false,
  },
  {
    id: 3,
    title:
      "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Amet maxime commodi doloremautem error, cumque facere similique aliquid adipisci a",
    status: false,
  },
]);

const handleClick = (id) => {
  const find = data.find((obj) => obj.id === id);
  if (find) {
    find.status = !find.status;
  }
};
</script>

<style scoped>
.accordion {
  width: 500px;
  max-width: 600px;
  margin: 0 auto;
}

.accordion-item {
  width: 500px;
  border: 1px solid #ddd;
  margin-bottom: 5px;
  border-radius: 4px;
  overflow: hidden;
}

.accordion-header {
  background-color: #f5f5f5;
  padding: 15px;
  margin: 0;
  cursor: pointer;
  font-size: 16px;
  font-weight: bold;
}

.accordion-header:hover {
  background-color: #e9e9e9;
}

.accordion-content {
  padding: 15px;
}
</style>
