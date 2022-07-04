<template>
  <section>
    <div class="wrapper">
      <br>
      <h1>Login Page</h1>
      <form>
        <div class="from-group">
          <input type="text" class="form-control">
        </div>
        <br>
        <p>
          <nuxt-link class="nuxt_link" to="/">To Home Page</nuxt-link>
        </p>
        <button class="btn btn-primary" type="submit">Login</button>
      </form>
    </div>
  </section>
</template>

<script>
export default {
  name: "login",
  layout: 'empty'
}
</script>

<style scoped lang="scss">
.wrapper{
  margin: 0 auto;
  background-color: #3f3f40;
  height: 1800px;
  input{
    background-color: wheat;
  }
}
.nuxt_link{
  text-decoration: none;
  font-weight: bold;
}
h1{
  color: wheat;
}
form{
  width: 500px;
}
</style>
