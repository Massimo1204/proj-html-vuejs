<template>
  <section class="text-uppercase">
    <indexHeader :navbarItems="navbarItems" />
    <div class="jumbo-text-wrapper d-flex flex-column justify-content-center">
      <div class="my-subtitle-wrapper">
        <div class="green-line d-inline-block"></div>
        <span class="my-subtitle">Alwats the best way you need it</span>
      </div>
      <div>
        <h1 class="my-title my-title-large">the best business consulting</h1>
      </div>
      <div class="jumbo-btn-wrapper d-flex">
        <button class="my-button my-button-green">read more</button>
        <div class="d-inline-block align-self-end">
          <span>
            <i class="fa-solid fa-play"></i>
          </span>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import indexHeader from "./Header.vue";
export default {
  name: "indexJumbo",
  components: {
    indexHeader,
  },
  props: ["navbarItems"],
};
</script>

<style lang="scss" scoped>
@import "../style.scss";

section {
  padding: 0 $my-offset;
  background-image: url("../assets/jumbotron-image.jpg");
  background-position-y: top;
  background-position-x: right;
  background-repeat: no-repeat;
  background-color: $bg-dark-blue;
  height: 100vh;
  div.jumbo-text-wrapper {
    height: calc(100vh - 100px);
    width: 60%;
    div.jumbo-btn-wrapper {
      div {
        margin: 10px 0 0 40px;
        padding: 12px 18px 15px 22px;
        border: 2px solid white;
        border-radius: 50%;
        span {
          filter: brightness(0) saturate(100%) invert(76%) sepia(30%)
            saturate(888%) hue-rotate(104deg) brightness(104%) contrast(104%);
        }
      }
    }
  }
}
</style>
