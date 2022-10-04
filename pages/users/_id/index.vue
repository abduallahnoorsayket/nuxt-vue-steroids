<template>
  <div>
    <h1>The user ID page, with ID: {{ $route.params.id }}</h1>
  </div>
</template>

<script>
export default {
  validate(data) {
    // console.log("10===", data);
    return /^\d+$/.test(data.params.id);
  },
};
</script>

<style></style>
