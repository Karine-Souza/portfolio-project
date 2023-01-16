<template>
  <div class="layout">
    <P_Header />
    <P_Latest_work />
    <P_Banner />
    <P_Testimonials />
    <P_Footer />
  </div>
</template>

<script>
import P_Header from "../components/organisms/P_Header";
import P_Latest_work from "../components/organisms/P_Latest_work";
import P_Banner from "../components/molecules/P_Banner";
import P_Testimonials from "../components/organisms/P_Testimonials";
import P_Footer from "../components/organisms/P_Footer";

export default {
  components: {
    P_Header,
    P_Latest_work,
    P_Banner,
    P_Testimonials,
    P_Footer,
  },
};
</script>
