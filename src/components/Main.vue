<template>
  <main>
    <helpSection />
    <aboutUsSection />
    <projectSection />
    <testimonialSection />
    <recentSection />
  </main>
</template>

<script>
import helpSection from "./sections/HelpSection.vue";
import aboutUsSection from "./sections/AboutUs.vue";
import projectSection from "./sections/Project.vue";
import testimonialSection from "./sections/Testimonial.vue";
import recentSection from "./sections/Recent.vue";

export default {
  name: "indexMain",
  components: {
    helpSection,
    aboutUsSection,
    projectSection,
    testimonialSection,
    recentSection,
  },
};
</script>

<style lang="scss" scoped></style>
