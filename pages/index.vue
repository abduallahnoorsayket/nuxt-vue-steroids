<template>
  <section class="container">
    <h1>This is the Main index page.</h1>
    <nuxt-link to="/users">Users page</nuxt-link>
    <button @click="onLoadProducts">Products</button>
  </section>
</template>

<script>
export default {
  name: "IndexPage",
  methods: {
    onLoadProducts() {
      this.$router.push("/products");
    },
  },
};
</script>
<style scoped>
/* .productRoute {
  text-decoration: none !important;
} */
</style>
