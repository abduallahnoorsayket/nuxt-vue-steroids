<template>
  <div>
    <h1>This is users index</h1>
    <input type="text" v-model="userId" />
    <button @click="onLoadUser">Load User</button>
    <nuxt-child />
  </div>
</template>

<script>
export default {
  data() {
    return {
      userId: "",
    };
  },
  layout: "usersLayout",
  methods: {
    onLoadUser() {
      this.$router.push("/users/" + this.userId);
    },
  },
};
</script>

<style></style>
