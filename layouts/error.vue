<template>
  <div class="container d-flex justify-content-center align-items-center">
    <div v-if="error.statusCode === 404" class="">
      <b-img fluid src="https://httpstatusdogs.com/img/404.jpg" alt=""></b-img>
    </div>
    <div v-else-if="error.statusCode === 400" class="">
      <b-img fluid src="https://httpstatusdogs.com/img/400.jpg" alt=""></b-img>
    </div>
    <div v-else-if="error.statusCode === 401" class="">
      <b-img fluid src="https://httpstatusdogs.com/img/401.jpg" alt=""></b-img>
    </div>
    <div v-else-if="error.statusCode === 402" class="">
      <b-img fluid src="https://httpstatusdogs.com/img/402.jpg" alt=""></b-img>
    </div>
    <div v-else-if="error.statusCode === 405" class="">
      <b-img fluid src="https://httpstatusdogs.com/img/405.jpg" alt=""></b-img>
    </div>
    <div v-else-if="error.statusCode === 403" class="">
      <b-img fluid src="https://httpstatusdogs.com/img/403.jpg" alt=""></b-img>
    </div>
    <div v-else class="">
      <b-img fluid src="https://support.apple.com/library/content/dam/edam/applecare/images/fr_FR/macos/Mojave/macos-mojave-restart-problem-ignore-report-alert.jpg" alt=""></b-img>
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
