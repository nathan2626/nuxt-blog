<template>
  <div class="container d-flex justify-content-center align-items-center">
    <div class="">
      <b-img fluid src="https://httpstatusdogs.com/img/404.jpg" alt=""></b-img>
    </div>
  </div>
</template>

<script>
export default {
  name: "error",
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

<style scoped>

</style>
