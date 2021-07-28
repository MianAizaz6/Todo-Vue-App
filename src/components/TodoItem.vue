<template>
  <div class="todo-item" v-bind:class="{ 'is-complete': todo.completed }">
    <h2>{{ todo.Title }}</h2>
  </div>
</template>

<script>
export default {
  name: "TodoItem",
  props: ["todo"],
};
</script>

<style scoped>
.todo-item {
  background-color: antiquewhite;
  padding: 10px;
  border-bottom: 1px grey dotted;
}
.is-complete {
  text-decoration: line-through;
}
.del {
  background-color: red;
  color: white;
  padding: 5px 9px;
  border: none;
  border-radius: 50%;
  cursor: pointer;
  float: right;
}
</style>