<template>
  <Banner />
  <CustomerCare />
  <AboutMe />
  <OurServices />
  <OurProject />
  <Achievement />
</template>

<script>
import Banner from "../components/home/Banner.vue";
import CustomerCare from "~/components/home/CustomerCare.vue";
import AboutMe from "../components/home/AboutMe.vue";
import OurServices from "../components/home/OurServices.vue";
import OurProject from "../components/home/OurProject.vue";
import Achievement from "../components/home/Achievement.vue";

export default {
  components: {
    Banner,
    CustomerCare,
    AboutMe,
    OurServices,
    OurProject,
    Achievement,
  },
};
</script>

<style>
</style>