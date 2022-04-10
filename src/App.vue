<template>
  <div id="app">
    <indexJumbo :navbarItems="navbarItems" />
  </div>
</template>

<script>
import indexJumbo from "./components/Jumbotron.vue";

export default {
  name: "App",
  components: {
    indexJumbo,
  },
  data: function () {
    return {
      navbarItems: [
        {
          name: "home",
          url: "#",
        },
        {
          name: "about",
          url: "#",
        },
        {
          name: "projects",
          url: "#",
        },
        {
          name: "services",
          url: "#",
        },
        {
          name: "blog",
          url: "#",
        },
        {
          name: "contact",
          url: "#",
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
}
</style>
