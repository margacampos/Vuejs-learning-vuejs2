<!-- eslint-disable prettier/prettier -->
<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link :to="'/'+route">{{ route }}</router-link>
  </nav>
</template>
<!-- eslint-disable prettier/prettier -->
<script>
export default {
  props:['route'],
  data: () => {
    return {
      
    };
  },
};
</script>
<!-- eslint-disable prettier/prettier -->
<style scoped>
nav { 
  background-color: black;
  padding: 30px;
}  
nav a { 
  color: white;
  font-weight: bold; 
}
nav a.router-link-exact-active {
  color: #42b983;
}
</style>
