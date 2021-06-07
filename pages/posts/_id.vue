<template>
  <div class="container">
    <Navbar />
    <div>
      <Post :post="post"></Post>
    </div>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: this.post.title
    }
  },
  data() {
    return {
      post: {}
    }
  },
  async asyncData({ params, $axios }) {
    const post = await $axios.$get(`https://jsonplaceholder.typicode.com/posts/${params.id}`);
    return {
      post
    }
  },
  name: "_id",

}
</script>

<style scoped>

</style>
