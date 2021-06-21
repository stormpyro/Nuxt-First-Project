<template>
  <div class="card">
    <h2>{{ post.title }}</h2>
    <p>ID: {{ post.id }}</p>
    <p>UserID: {{ post.userId }}</p>
    <p>Content: {{ post.body }}</p>
  </div>
</template>
<script>
export default {
  data: () => ({
    post: {},
  }),
  created: async function () {
    this.post = await this.$axios.$get(
      "https://jsonplaceholder.typicode.com/posts/" + this.$route.params.id
    );
  },
};
</script>
<style>
.card {
  border: 1px solid whitesmoke;
  padding: 4rem;
}
</style>