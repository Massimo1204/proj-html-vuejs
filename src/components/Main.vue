<template>
  <main>
    <helpSection />
    <aboutUsSection />
  </main>
</template>

<script>
import helpSection from "./sections/HelpSection.vue";
import aboutUsSection from "./sections/AboutUs.vue";
export default {
  name: "indexMain",
  components: {
    helpSection,
    aboutUsSection,
  },
};
</script>

<style lang="scss" scoped></style>
