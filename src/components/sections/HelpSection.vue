<template>
  <section>
    <div class="title-wrapper position-relative">
      <h3 class="my-title d-inline-block">our consultants can help you</h3>
      <div class="green-line d-inline-block position-absolute"></div>
    </div>
    <div
      class="help-content-wrapper d-flex flex-column justify-content-between"
    >
      <div class="d-flex justify-content-between w-100">
        <div class="help-text-wrapper d-flex align-items-start">
          <img src="../../assets/graph.png" alt="graph icon" />
          <div class="d-inline-block">
            <h4 class="my-title">statistical consulting</h4>
            <p>
              When, while lovely valley teems with vapour around meand eridian
              sun strikes the upper impenetrable foliage of my trees, and but a
            </p>
          </div>
        </div>
        <div class="help-text-wrapper d-flex align-items-start">
          <img src="../../assets/megaphone.png" alt="megaphone icon" />
          <div class="d-inline-block">
            <h4 class="my-title">digital consulting</h4>
            <p>
              When, while lovely valley teems with vapour around meand eridian
              sun strikes the upper impenetrable foliage of my trees, and but a
            </p>
          </div>
        </div>
      </div>
      <div class="d-flex justify-content-between w-100">
        <div class="help-text-wrapper d-flex align-items-start">
          <img src="../../assets/wallet.png" alt="wallet icon" />
          <div class="d-inline-block">
            <h4 class="my-title">banking consulting</h4>
            <p>
              When, while lovely valley teems with vapour around meand eridian
              sun strikes the upper impenetrable foliage of my trees, and but a
            </p>
          </div>
        </div>
        <div class="help-text-wrapper d-flex align-items-start">
          <img src="../../assets/bullseye.png" alt="bullseye icon" />
          <div class="d-inline-block">
            <h4 class="my-title">enterprise consulting</h4>
            <p>
              When, while lovely valley teems with vapour around meand eridian
              sun strikes the upper impenetrable foliage of my trees, and but a
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
};
</script>

<style lang="scss" scoped>
@import "../../style.scss";
section {
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
      }
    }
    div {
      width: 500px;
    }
  }
}
</style>
