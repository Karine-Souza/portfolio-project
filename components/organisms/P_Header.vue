<template>
  <div class="header">
    <P_Menu />
    <P_Hero_image
      class="Header__banner"
      :link="'ABOUT'"
      :titulo="'An Experience Design Agency'"
      :subtitulo="'Provides a full service range'"
      :texto="`Ability to put themselves in the merchant's shoes. It is meant to
          partner on the long run, and work as an extension of the merchant's
          team.`"
      :src="require('@/assets/images/pic (3).png')"
    />
  </div>
</template>

<script>
import P_Menu from "../molecules/P_Menu.vue";
import P_Hero_image from "../molecules/P_Hero_image.vue";

export default {
  components: {
    P_Menu,
    P_Hero_image,
  },
};
</script>

<style lang="scss">
.header {
  &__banner {
    .heroImage__container {
      .heroImage__textSide {
        margin: 0;
      }
      .heroImage__imageSide {
        @media (min-width: 992px) {
          .heroImage__image {
            width: 446px;
            height: 565px;
          }
        }
        @media (min-width: 1280px) {
          .heroImage__image {
            width: 566px;
            height: 585px;
          }
        }
      }
    }
  }
}
</style>
