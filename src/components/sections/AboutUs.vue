<template>
  <section ref="aboutUs">
    <div class="main-part d-flex justify-content-end align-items-center">
      <div class="main-part-text">
        <div class="my-subtitle-wrapper">
          <div class="green-line d-inline-block"></div>
          <span class="my-subtitle">About Us</span>
        </div>
        <div>
          <h2 class="my-title">we make your strategy work</h2>
          <p>
            When, while lovely valley teems with vapour around meand eridian sun
            strikes the upper impenetrable foliage of my trees, and but a
            thousand unknown plants are noticed when I hear the buzz of the
            little world among the stalks,and grow familiar indescribable forms
            of the insects.and flies, then I feel the presence of the Almighty.
          </p>
        </div>
      </div>
    </div>
    <div class="aboutUs-bottom-part position-relative">
      <div class="aboutUs-bottom-text-wrapper d-flex align-items-center h-100">
        <div class="d-flex justify-content-between w-100">
          <h2 class="my-title m-0">we help to deliver the business case</h2>
          <p class="m-0">
            When, while lovely valley teems with vapour around meand meridian
            sun strikes the upper impenetrable foliage of my trees, and but a
            thousand unknown
          </p>
        </div>
      </div>
      <div class="position-absolute aboutUs-button-wrapper">
        <button class="my-button my-button-red">get started</button>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "aboutUsSection",
};
</script>

<style lang="scss" scoped>
@import "../../style.scss";

section {
  margin-right: $my-offset;
  div.main-part {
    background-image: url("../../assets/business-people-working-together-on-project.jpg");
    background-position-x: left;
    background-position-y: top;
    background-repeat: no-repeat;
    background-size: 60%;
    height: 824px;
    div.main-part-text {
      width: 522px;
      margin-right: 90px;
      div {
        h2 {
          font-size: 3.75rem;
          line-height: 4rem;
          margin-bottom: 2.7rem;
        }
        p {
          color: rgb(157, 158, 167);
          font-weight: 500;
        }
      }
    }
  }
  div.aboutUs-bottom-part {
    padding: 0 20vw 0 $offset-large;
    height: 323px;
    background-color: $my-green;
    color: black;
    div.aboutUs-bottom-text-wrapper {
      padding-top: 30px;
      color: $bg-dark-blue;
      h2 {
        width: 375px;
        font-size: 2.2rem;
        line-height: 2.7rem;
        letter-spacing: -2px;
      }
      p {
        width: 430px;
      }
    }
    div.aboutUs-button-wrapper {
      right: 0;
      bottom: 0;
      button.my-button {
        padding: 20px 50px;
      }
    }
  }
}
</style>
