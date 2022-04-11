<template>
  <main>
    <helpSection />
    <aboutUsSection />
    <projectSection />
    <testimonialSection />
  </main>
</template>

<script>
import helpSection from "./sections/HelpSection.vue";
import aboutUsSection from "./sections/AboutUs.vue";
import projectSection from "./sections/Project.vue";
import testimonialSection from "./sections/Testimonial.vue";

export default {
  name: "indexMain",
  components: {
    helpSection,
    aboutUsSection,
    projectSection,
    testimonialSection,
  },
};
</script>

<style lang="scss" scoped></style>
