<template>
  <section>
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
    height: 844px;
    div.main-part-text {
      width: 500px;
      margin-right: 50px;
      div {
        h2 {
          font-size: 3.75rem;
          line-height: 4rem;
          margin-bottom: 3rem;
        }
        p {
          color: grey;
        }
      }
    }
  }
}
</style>
