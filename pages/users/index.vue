<template>
  <section>
    <h1>Users page</h1>
    <ul>
      <li
        v-for="user of 5" :key="user">
        <a href="#" @click.prevent="openUser(user)">User {{ user }}</a>
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  name: "index",
  methods: {
    openUser(user) {
      this.$router.push('/users/'+ user)
    }
  }
}
</script>

<style scoped lang="scss">
section{
  height: 1800px;
  color: wheat;
  background-color: #3f3f40;
    h1{
      margin-left: 50px;
    }
    ul{
      margin-left: 50px;
    }
}
</style>
