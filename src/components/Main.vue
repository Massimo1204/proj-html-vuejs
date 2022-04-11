<template>
  <main>
    <helpSection />
    <aboutUsSection />
    <projectSection />
  </main>
</template>

<script>
import helpSection from "./sections/HelpSection.vue";
import aboutUsSection from "./sections/AboutUs.vue";
import projectSection from "./sections/Project.vue";
export default {
  name: "indexMain",
  components: {
    helpSection,
    aboutUsSection,
    projectSection,
  },
};
</script>

<style lang="scss" scoped></style>
