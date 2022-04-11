<template>
  <section>
    <div class="my-subtitle-wrapper">
      <div class="green-line d-inline-block"></div>
      <span class="my-subtitle">project</span>
    </div>
    <div class="project-title-wrapper d-flex justify-content-between">
      <h2 class="my-title my-title-medium">
        our expert trusted consultants help clients
      </h2>
      <div class="project-arrows-wrapper">
        <div class="project-arrow-wrapper">
          <i class="fas fa-arrow-left-long"></i>
        </div>
        <div class="project-arrow-wrapper ms-2">
          <i class="fas fa-arrow-right-long"></i>
        </div>
      </div>
    </div>
    <div class="project-images-wrapper">
      <img src="" alt="" />
    </div>
  </section>
</template>

<script>
export default {
  name: "projectSection",
  data: function () {
    return {};
  },
};
</script>

<style lang="scss" scoped>
@import "../../style.scss";

section {
  height: 976px;
  padding: 200px 8vw 0 8vw;
  div.my-subtitle-wrapper {
    margin-bottom: 1.5rem;
  }
  div.project-title-wrapper {
    h2.my-title {
      width: 60%;
    }
    div.project-arrows-wrapper {
      padding-top: 20px;
      div.project-arrow-wrapper {
        padding: 17px 20px 13px 20px;
        background-color: rgba($color: #ffffff, $alpha: 0.1);
        display: inline-block;
      }
    }
  }
}
</style>
