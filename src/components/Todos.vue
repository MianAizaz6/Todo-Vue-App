<template>
  <h2>This is Todos Component</h2>
  <div v-bind:key="todo.id" v-for="todo in todos">
    <TodoItem v-bind:todo="todo" />
  </div>
</template>


<script>
import TodoItem from "./TodoItem.vue";

export default {
  name: "Todos",
  components: {
    TodoItem,
  },
  props: ["todos"],
};
</script>

<style scoped>
</style>