<template>
  <footer>
    <div
      class="getStarted d-flex justify-content-center align-items-center flex-column"
    >
      <h2 class="my-title my-title-medium">let's talk about work</h2>
      <div class="getStarted-text-wrapper text-center">
        <p>
          A wonderful serenity has taken possession Far far away, behind the
          word mountains.
        </p>
        <button class="my-button">get started</button>
      </div>
    </div>
    <div class="bottom-footer">
      <div
        class="footer-nav-wrapper d-flex justify-content-between align-items-center"
      >
        <img src="../assets/logotype-2.png" alt="phlox logo" />
        <ul>
          <li
            v-for="(element, index) in navbarItems"
            :key="index + 'footer-nav'"
          >
            <a :href="element.url">{{ element.name }}</a>
          </li>
        </ul>
        <div class="socials">
          <i
            class="ms-4"
            v-for="(element, index) in socials"
            :key="index + 'social'"
            :class="element"
          ></i>
        </div>
      </div>
      <div
        class="footer-info d-flex justify-content-between position-relative align-items-center"
      >
        <div>
          <p class="m-0">Terms of use</p>
          <p class="text-capitalize">Privacy environmental policy</p>
        </div>
        <p class="text-capitalize">
          Copyright &#169; 2020 phlox consulting.all rights reserved.
        </p>
        <div href="#" class="position-absolute arrow-up">
          <i class="fas fa-arrow-up-long"></i>
        </div>
        <div class="position-absolute comment-icon">
          <i class="fa-regular fa-comment"></i>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "indexFooter",
  props: ["navbarItems"],
  data: function () {
    return {
      socials: [
        "fab fa-instagram",
        "fab fa-linkedin-in",
        "fab fa-facebook-f",
        "fab fa-twitter",
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style.scss";
footer {
  div.getStarted {
    padding-top: 55px;
    height: 460px;
    background-image: url("../assets/footer-bg.jpg");
    background-position: center;
    h2.my-title {
      margin-bottom: 0.4rem;
    }
    div.getStarted-text-wrapper {
      width: 25%;
      p {
        color: rgb(216, 207, 207);
        margin-bottom: 1.6rem;
        font-size: 1.1rem;
      }
      button {
        background-color: $bg-dark-blue;
        color: white;
      }
    }
  }
  div.bottom-footer {
    height: 310px;
    padding: 0 $my-offset 50px $my-offset;
    div.footer-nav-wrapper {
      height: 190px;
      border-bottom: 1px solid rgba(90, 88, 88, 0.5);
      img {
        height: 25px;
      }
      ul {
        list-style: none;
        padding-right: 10px;
        li {
          display: inline;
          a {
            text-decoration: none;
            color: grey;
            margin: 0 10px;
            text-transform: uppercase;
          }
        }
      }
    }
    div.footer-info {
      height: 120px;
      padding-top: 20px;
      color: grey;
      font-size: 0.9rem;
      div.arrow-up {
        bottom: 48%;
        left: 100.6%;
        background-color: white;
        padding: 8px 13px 8px 13px;
        font-size: 0.67rem;
        border-radius: 50%;
      }
      div.comment-icon {
        font-size: 1.6rem;
        bottom: 35%;
        left: 104%;
        color: white;
        background-color: rgb(82, 124, 235);
        padding: 9px 17px 13px 17px;
        border-radius: 50%;
      }
    }
  }
}
</style>
