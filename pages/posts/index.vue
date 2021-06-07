<template>
  <div class="container">
    <Navbar />
    <div>
      <Posts :posts="posts" />
    </div>
  </div>
</template>

<script>

export default {
  data() {
    return {
      posts: []
    }
  },
  async asyncData({ params, $axios }) {
    const posts = await $axios.$get(`https://jsonplaceholder.typicode.com/posts`);
    console.log(posts)
    return {
      posts
    }
  },
  name: "index",
  head: {
    titleTemplate: '%s - Nuxt.js',
    meta: [
      { charset: 'utf-8' },
      { name: 'viewport', content: 'width=device-width, initial-scale=1' },

      // hid is used as unique identifier. Do not use `vmid` for it as it will not work
      { hid: 'description', name: 'description', content: 'Meta description' }
    ]
  },
}
</script>

