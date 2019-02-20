<template>
  <div class="home">
    <Todos msg="Welcome to My Vue.js Todo App" :todos="todos"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Todos from "@/components/Todos.vue";

export default {
  name: "todos",
  components: {
    Todos
  },
  data: () => {
    return { todos: [{ id: 1, title: "1sts", body: "1st notes body 🙉" }] };
  }
};
</script>
