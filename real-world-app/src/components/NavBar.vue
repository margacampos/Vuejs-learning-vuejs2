<!-- eslint-disable prettier/prettier -->
<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/heyyy">{{ route }}</router-link>
  </nav>
</template>
<!-- eslint-disable prettier/prettier -->
<script>
export default {
  data: () => {
    return {
      route: "hola",
    };
  },
};
</script>
<!-- eslint-disable prettier/prettier -->
<style></style>
