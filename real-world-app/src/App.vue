<template>
  <div id="app">
    <NavBar :route="route" />
    <Form :route="route" @change-route="(r) => changeRoute(r)" />
    <router-view />
  </div>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import Form from "./components/NameForm.vue";

export default {
  components: {
    NavBar,
    Form,
  },
  data: () => {
    return {
      route: "World",
    };
  },
  methods: {
    changeRoute(r) {
      console.log("happened");
      this.route = r;
    },
  },
};
</script>
<style>
html {
  display: inline-block;
  margin: 0;
  padding: 0;
}

body {
  margin: 0;
  padding: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
