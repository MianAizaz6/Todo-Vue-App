<template>
  <Todos v-bind:todos="todos" />
</template>

<script>
import Todos from "./components/Todos.vue";
export default {
  name: "App",
  components: {
    Todos,
  },
  data() {
    return {
      todos: [
        {
          id: 1,
          Title: "Do Homework",
          completed: false,
        },
        {
          id: 2,
          Title: "Go For Excersie",
          completed: true,
        },
        {
          id: 3,
          Title: "Go to Bed",
          completed: false,
        },
      ],
    };
  },
};
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  pad: 0;
}
body {
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
  line-height: 1.4;
}
</style>
