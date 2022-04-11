<template>
  <section>
    <div class="title-wrapper position-relative">
      <h3 class="my-title d-inline-block">our consultants can help you</h3>
      <div class="green-line d-inline-block position-absolute"></div>
    </div>
    <div
      class="help-content-wrapper d-flex flex-column justify-content-between"
    >
      <div
        class="d-flex justify-content-between w-100"
        v-for="(items, index) in helpSectionItems"
        :key="index"
      >
        <div
          class="help-text-wrapper d-flex align-items-start"
          v-for="(element, index) in items"
          :key="index + 'inside'"
        >
          <img
            :src="require(`../../assets/${element.imgSrc}`)"
            :salt="element.name"
          />
          <div class="d-inline-block">
            <h4 class="my-title">{{ element.title }}</h4>
            <p>
              {{ element.description }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "helpSection",
  data: function () {
    return {
      helpSectionItems: [
        [
          {
            title: "statistical consulting",
            name: "graph icon",
            imgSrc: "graph.png",
            description:
              "When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a",
          },
          {
            title: "digital consulting",
            name: "megaphone icon",
            imgSrc: "megaphone.png",
            description:
              "When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a",
          },
        ],
        [
          {
            title: "banking consulting",
            name: "wallet icon",
            imgSrc: "wallet.png",
            description:
              "When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a",
          },
          {
            title: "enterprise consulting",
            name: "graph icon",
            imgSrc: "bullseye.png",
            description:
              "When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a",
          },
        ],
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../../style.scss";
section {
  overflow-x: hidden;
  background-color: white;
  color: black;
  padding: $my-offset $offset-large 200px $offset-large;
  div.title-wrapper {
    margin-bottom: $my-offset;
    h3.my-title {
      margin: 0 50px 0 0;
    }
    div.green-line {
      width: 70vw;
      top: 50%;
      transform: translateY(-50%);
    }
  }
  div.help-content-wrapper {
    height: 390px;
    div.help-text-wrapper {
      img {
        margin-right: 40px;
      }
      div {
        margin-top: 10px;
        h4 {
          margin-bottom: 1rem;
        }
        p {
          color: rgb(78, 78, 80);
        }
      }
    }
    div {
      width: 500px;
    }
  }
}
</style>
