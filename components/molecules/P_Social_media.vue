<template>
  <div class="socialMedia">
    <a target="_blank" href="https://www.facebook.com"
      ><P_Icon
        :icon-src="require('@/assets/icons/orange_sm_facebook.png')"
        :icon-alt="'Facebook'"
        class="socialMedia__icon socialMedia__facebook"
    /></a>
    <a target="_blank" href="https://www.twitter.com/">
      <P_Icon
        :icon-src="require('@/assets/icons/orange_sm_twitter.png')"
        :icon-alt="'Twitter'"
        class="socialMedia__icon socialMedia__twitter"
    /></a>
    <a target="_blank" href="https://www.instagram.com/">
      <P_Icon
        :icon-src="require('@/assets/icons/orange_sm_instagram.png')"
        :icon-alt="'Instagram'"
        class="socialMedia__icon socialMedia__instagram"
    /></a>
  </div>
</template>

<script>
import P_Icon from "../atoms/P_Icon.vue";

export default {
  components: {
    P_Icon,
  },
};
</script>

<style lang="scss">
.socialMedia {
  position: relative;
  display: flex;
  margin-left: 10px;
  justify-content: space-between;
  width: 160px;
}
</style>
