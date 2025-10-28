<template>
  <div class="task-item">
    <h3>{{ task.title }}</h3>
    <p>{{ task.text }}</p>
  </div>
</template>

<script setup>
defineProps({
  task: {
    type: Object,
    required: true
  }
})
</script>

<style scoped>
.task-item {
  border: 1px solid #ccc;
  border-radius: 8px;
  padding: 16px;
  margin-bottom: 12px;
  background-color: #f9f9f9;
}
.task-item h3 {
  margin: 0 0 8px;
  color: #333;
}
.task-item p {
  margin: 0;
  color: #666;
}
</style>
