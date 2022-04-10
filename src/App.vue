<template>
  <div id="app">
    <indexJumbo :navbarItems="navbarItems" />
    <indexMain />
  </div>
</template>

<script>
import indexJumbo from "./components/Jumbotron.vue";
import indexMain from "./components/Main.vue";

export default {
  name: "App",
  components: {
    indexJumbo,
    indexMain,
  },
  data: function () {
    return {
      navbarItems: [
        {
          name: "home",
          url: "#",
          state: true,
        },
        {
          name: "about",
          url: "#",
          state: false,
        },
        {
          name: "projects",
          url: "#",
          state: false,
        },
        {
          name: "services",
          url: "#",
          state: false,
        },
        {
          name: "blog",
          url: "#",
          state: false,
        },
        {
          name: "contact",
          url: "#",
          state: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "./style.scss";
#app {
  font-family: "Montserrat", sans-serif;
  color: white;
  min-width: 1550px;
  background-color: $bg-dark-blue;
}
</style>
