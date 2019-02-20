<template>
  <div key="id" class="notes-list--cardcontainer">
    <h1>{{ title }}</h1>
    <p>{{ body }}</p>
  </div>
</template>

<script>
export default {
  name: "TodoCard",
  props: {
    title: String,
    body: String,
    id: Number
  }
};
</script>

<style scoped>
.notes-list--cardcontainer {
  border: 1px solid black;
  width: 60%;
  margin: 0 auto;
}
</style>
