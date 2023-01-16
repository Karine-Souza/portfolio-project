<template>
  <div class="banner">
    <P_Hero_image
      class="banner__text"
      :link="'ABOUT'"
      :titulo="'An Experience Webflow Expert'"
      :subtitulo="'Provides a full service range'"
      :texto="`Ability to put themselves in the merchant's shoes. It is meant to partner on the long run, and work as an extension of the merchant's team.`"
      :backgroundColor="'#28293E'"
      :src="require('@/assets/images/pic (5).png')"
    />
  </div>
</template>

<script>
import P_Hero_image from "../molecules/P_Hero_image.vue";
import P_Button from "../atoms/P_Button.vue";

export default {
  components: {
    P_Hero_image,
    P_Button,
  },
};
</script>

<style lang="scss">
.banner {
  h1 {
    color: #ffffff;
  }

  h5 {
    color: #ffffff;
  }

  p {
    color: rgba(255, 255, 255, 0.64);
  }
  .heroImage__container {
  }
}
</style>
