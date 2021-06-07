<template>
  <nav class="mt-5 mb-5 navbar navbar-expand-lg navbar-light bg-light">
    <nuxt-link to="/">
      Blog
    </nuxt-link>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarText" aria-controls="navbarText" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarText">
      <ul class="navbar-nav mr-auto">
        <li class="nav-item">
          <nuxt-link  class="nav-link" to="/about">
            About
          </nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link  class="nav-link" to="/posts">
            Posts
          </nuxt-link>
        </li>
      </ul>
      <span class="navbar-text">
      © Blog des Posts Natan (officieusement)
    </span>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Navbar"
}
</script>

<style scoped>

</style>
