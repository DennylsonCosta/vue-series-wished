<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">

    <router-link
      class="navbar-brand"
      :to="{ name: 'home' }"
    >
      Series Wished
    </router-link>

    <div class="collapse navbar-collapse">
      <ul class="navbar-nav mr-auto"> 
        <li class="nav-item active">
          <a class="nav-link" href="#">Home</a>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  computed: {
    routes () {
      return this.$router.options.routes.filter(route => (
        route.meta && route.meta.showNavbar
      ))
    }
  }
}
</script>

<style>

</style>
