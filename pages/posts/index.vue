<template>
  <div>
    <h1>Posts</h1>
    <Post
      v-for="(item, index) in posts"
      :key="index"
      :name="item.title"
      :id="item.id"
    />
  </div>
</template>
<script>
import Post from "../../components/Post.vue";
export default {
  data: () => ({
    posts: [],
  }),
  components: {
    Post,
  },
  created: async function () {
    const data = await this.$axios.$get(
      "https://jsonplaceholder.typicode.com/posts"
    );
    this.posts = data;
  },
};
</script>