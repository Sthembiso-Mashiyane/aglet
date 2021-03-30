<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-transparent">
    <router-link to="/"><img src="../../assets/aglet_logo.svg" class="img-fluid" alt="">
    </router-link>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav mr-auto">

      </ul>
      <ul>
        <router-link to="/">Home</router-link>
        |
        <router-link to="/contact">Contact</router-link>
      </ul>
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
