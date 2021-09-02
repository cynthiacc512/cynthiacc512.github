
<template>
  <div>
    <HeroSection />
    <WorkExperience />
    <Education />
    <ContactMe />
    <Footer />
  </div>
</template>

<script>
import HeroSection from "./components/HeroSection";
import WorkExperience from "./components/WorkExperience.vue";
import Education from "./components/Education.vue";
import ContactMe from "./components/ContactMe.vue";
import Footer from "./components/Footer.vue";
import "bootstrap/dist/css/bootstrap.css";

export default {
  name: "App",

  components: {
    HeroSection,
    WorkExperience,
    Education,
    ContactMe,
    Footer,
  },

  data: () => ({
    //
  }),
};
</script>

<style>
body {
  background: #272727;
  color: #fff;
}

@import "../src/assets/styles/style.css";
@import "../src/assets/styles/responsive.css";
</style>