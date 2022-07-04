<template>
  <section>
    <div class="wrapper"><br>
      <h1>Users page</h1>
      <ul>
        <li
          v-for="user of users" :key="user.id">
          <a href="#" @click.prevent="openUser(user)">User -- {{ user.name }}</a>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  data: () => ({
    users: []
  }),
  async mounted() {
    this.users = await this.$axios.$get('https://jsonplaceholder.typicode.com/users')
  },
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
}
.wrapper{
  background-color: #3f3f40;
}
</style>
