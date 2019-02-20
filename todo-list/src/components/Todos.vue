<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>Hi Hello, hi!</p>
    <NoteCard v-for="todo in todos" key="todo.id" :title="todo.title" :body="todo.body"/>
  </div>
</template>

<script>
import NoteCard from "@/components/NoteCard.vue";
export default {
  beforeMount() {
    console.log("Here I am 👋");
  },
  mounted() {
    console.log("Here go our API calls 😇");
  },
  name: "Todos",
  components: {
    NoteCard
  },
  props: {
    msg: String,
    todos: Array
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
