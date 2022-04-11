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
    <div class="project-images-wrapper d-flex justify-content-between w-100">
      <img
        v-for="(element, index) in projectImages"
        :key="index"
        :src="require(`../../assets/${element.imgSrc}`)"
        :alt="element.name"
      />
    </div>
  </section>
</template>

<script>
export default {
  name: "projectSection",
  data: function () {
    return {
      projectImages: [
        {
          name: "dry image",
          imgSrc: "dry.jpg",
        },
        {
          name: "sponsorship image",
          imgSrc: "sponsorship-proposal.jpg",
        },
        {
          name: "vizeion image",
          imgSrc: "consulting-vizeon.jpg",
        },
      ],
    };
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
        padding: 17px 19px 12px 19px;
        background-color: rgba($color: #ffffff, $alpha: 0.1);
        display: inline-block;
        filter: brightness(0.8);
      }
    }
  }
  div.project-images-wrapper {
    img {
      width: 32%;
      height: 380px;
    }
  }
}
</style>
