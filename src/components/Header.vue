<template>
  <header class="d-flex justify-content-between align-items-center">
    <img src="../assets/logotype.png" alt="" />
    <nav>
      <ul>
        <li v-for="(element, index) in navbarItems" :key="index">
          <a
            :class="element.state ? 'active' : ''"
            :href="element.url"
            @click="selectLink(index)"
          >
            {{ element.name }}
          </a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "indexHeader",
  props: ["navbarItems"],
  methods: {
    selectLink(i) {
      this.navbarItems.forEach((element, index) => {
        if (element.state) {
          element.state = false;
        } else if (index == i) {
          element.state = true;
        }
      });
    },
  },
};
</script>

<style scoped lang="scss">
header {
  height: 100px;
  img {
    height: 20px;
  }
  nav {
    ul {
      li {
        display: inline;
        a {
          text-decoration: none;
          color: lightgrey;
          margin-left: 33px;
          font-size: 0.9rem;
          padding: 31px 0;
        }
        a.active {
          color: white;
          font-weight: bold;
          border-top: 3px solid white;
        }
      }
    }
  }
}
</style>
