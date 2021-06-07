<template>
  <div>
    <p>{{post.title}}</p>
    <p>{{post.body}}</p>
  </div>
</template>

<script>
export default {
  props: [
    'post'
  ],
  name: "Post"
}
</script>

<style scoped>

</style>
