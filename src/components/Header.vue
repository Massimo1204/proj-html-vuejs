<template>
  <header class="d-flex justify-content-between align-items-center">
    <img src="../assets/logotype.png" alt="" />
    <nav>
      <ul>
        <li v-for="(element, index) in navbarItems" :key="index">
          <a :href="element.url"> {{ element.name }} </a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "indexHeader",
  props: ["navbarItems"],
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
          margin-left: 36px;
          font-size: 0.85rem;
        }
      }
    }
  }
}
</style>
