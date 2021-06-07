<template>
  <div v-if="posts.length">
    <ul v-for="post of posts" :key="post.id">
      <nuxt-link :to="`/posts/${post.id}`"> {{ post.title}}</nuxt-link>
    </ul>
  </div>
  <div v-else>
    No posts.
  </div>
</template>

<script>
export default {
  props: [
    'posts'
  ],
  name: "Posts"
}
</script>


