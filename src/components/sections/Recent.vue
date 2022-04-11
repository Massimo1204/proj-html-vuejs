<template>
  <section>
    <div class="recent-title-wrapper">
      <div class="my-subtitle-wrapper">
        <div class="green-line d-inline-block"></div>
        <span class="my-subtitle">blog</span>
      </div>
      <div class="clearfix w-100">
        <h2 class="my-title my-title-medium d-inline-block">
          the recent news you must read it
        </h2>
        <button class="my-button my-button-green float-end">view all</button>
      </div>
    </div>
    <div class="news-wrapper d-flex justify-content-between">
      <div
        class="new position-relative"
        v-for="(element, index) in recentNews"
        :key="index + 'news'"
      >
        <img
          class="img-fluid"
          :src="require(`../../assets/${element.imgSrc}`)"
          :alt="element.alt"
        />
        <div class="info position-absolute">
          <p class="date-author">
            <span class="new-date">{{ element.date }}</span
            ><span class="new-author ms-3">{{ element.name }}</span>
          </p>
          <h5 class="new-title my-title">{{ element.title }}</h5>
          <p class="new-text">{{ element.text }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "recentSection",
  data: function () {
    return {
      recentNews: [
        {
          alt: "startup image",
          imgSrc: "startup.jpg",
          date: "july 4, 2019",
          name: "by paul",
          title: "Canadian Consulting Film acquired by Uk Giant",
          text: "When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a ...",
        },
        {
          alt: "business image",
          imgSrc: "business.jpg",
          date: "july 4, 2019",
          name: "by paul",
          title: "Canadian Consulting Film acquired by Uk Giant",
          text: "When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a ...",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../../style.scss";
section {
  padding: 0 $my-offset 310px $my-offset;
  div.news-wrapper {
    div.new {
      width: 49%;
      div.info {
        width: 80%;
        height: 300px;
        right: 0;
        top: 65%;
        padding: 50px 160px 50px 80px;
        background-color: white;
        p.date-author {
          color: $my-red;
          font-weight: 500;
        }
        h5.new-title {
          color: black;
          font-size: 1.7rem;
          margin-bottom: 1.5rem;
          text-transform: none;
          font-weight: 500;
          letter-spacing: -2px;
        }
        p.new-text {
          color: darkgrey;
        }
      }
    }
  }
}
</style>
