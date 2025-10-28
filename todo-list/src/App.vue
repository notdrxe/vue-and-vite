<template>
  <div id="app">
    <h1>Список дел</h1>
    <TaskItem
      v-for="task in tasks"
      :key="task.id"
      :task="task"
    />
  </div>
</template>

<script setup>
import TaskItem from './components/TaskItem.vue'

const tasks = [
  { id: 1, title: 'Купить продукты', text: 'Молоко, хлеб, яйца' },
  { id: 2, title: 'Сделать домашку', text: 'Выучить стих' },
  { id: 3, title: 'Погулять с собакой', text: 'Выйти в 4 часа' },
  { id: 4, title: 'Прочитать книгу', text: 'Граф Монте Кристо' }

]
</script>

