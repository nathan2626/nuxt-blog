<template>
  <div class="container">
    <Navbar />

    <div>
      <b-img fluid src="/elizeu-dias-RN6ts8IZ4_0-unsplash.jpg" alt=""></b-img>
    </div>
  </div>
</template>

<script>
export default {
  head: {
    titleTemplate: '%s - Nuxt.js',
    meta: [
      { charset: 'utf-8' },
      { name: 'viewport', content: 'width=device-width, initial-scale=1' },

      // hid is used as unique identifier. Do not use `vmid` for it as it will not work
      { hid: 'description', name: 'description', content: 'Meta description' }
    ]
  }
}
</script>

