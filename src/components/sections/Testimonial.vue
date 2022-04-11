<template>
  <section>
    <div class="testimonial-title-wrapper clearfix">
      <div class="my-subtitle-wrapper position-relative text-center w-100">
        <span class="my-subtitle">testimonial</span>
        <div class="green-line d-inline-block position-absolute"></div>
      </div>
      <h2 class="my-title my-title-medium text-end float-end">
        what's the customer say about our work
      </h2>
    </div>
    <div class="reviews d-flex justify-content-between">
      <div
        class="review"
        v-for="(element, index) in reviewsList"
        :key="index + 'reviews'"
      >
        <p class="comment">{{ element.text }}</p>
        <h5 class="name fw-bold text-dark my-title">{{ element.name }}</h5>
        <p class="company m-0">{{ element.company }}</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "testimonialSection",
  data: function () {
    return {
      reviewsList: [
        {
          name: "Vera Duncan",
          company: "Amazon Inc.",
          text: "When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed by when I hear the buzz of the little .",
        },
        {
          name: "Vera Duncan",
          company: "Amazon Inc.",
          text: "When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed by when I hear the buzz of the little .",
        },
        {
          name: "Vera Duncan",
          company: "Amazon Inc.",
          text: "When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed by when I hear the buzz of the little .",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../../style.scss";

section {
  padding: 0 0 280px 8.5vw;
  div.testimonial-title-wrapper {
    padding-right: 8.7vw;
    div.my-subtitle-wrapper {
      margin-bottom: 0.5rem;
      div.green-line {
        right: 0;
        margin-right: 0;
      }
    }
    h2.my-title {
      width: 50%;
    }
  }
  div.reviews {
    background-color: white;
    padding: 50px calc(8.7vw + 60px) 75px 90px;
    div.review {
      width: 380px;
      p.comment {
        color: grey;
        margin-bottom: 3rem;
        font-size: 1.05rem;
      }
      h5.name {
        font-size: 1.6rem;
        margin-bottom: 0.7rem;
        text-transform: capitalize;
        letter-spacing: -2px;
      }
      p.company {
        color: darkgrey;
      }
    }
  }
}
</style>
