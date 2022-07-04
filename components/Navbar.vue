<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <ul class="navbar-nav mr-auto">
      <li class="nav-item nav-bar-left ">
        <ul class="navbar-nav mr-auto">
          <li class="nav-item">
            <nuxt-link no-prefetch exact active-class="active" to="/" class="nav-link">
              Home
            </nuxt-link>
          </li>
          <li class="nav-item">
            <nuxt-link active-class="active" to="/about" class="nav-link">
              About
            </nuxt-link>
          </li>
          <li class="nav-item">
            <nuxt-link active-class="active" to="/users" class="nav-link">
              Users
            </nuxt-link>
          </li>
          <li class="nav-item">
            <nuxt-link active-class="active" to="/login" class="nav-link">
              Login
            </nuxt-link>
          </li>
        </ul>
      </li>
    </ul>
    <div  class="nav-bar-right">
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent"
              aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <form class="form-inline my-2 my-lg-0">
          <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
          <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
        </form>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Navbar"
}
</script>

<style scoped lang="scss">
@import "./src/scss/navbar";


</style>
