<template>
  <div class="header">
    <P_Menu />
    <P_Hero_image
      class="Header__banner"
      :link="'About'"
      :titulo="'An Experience Design Agency'"
      :subtitulo="'Provides a full service range'"
      :texto="`Ability to put themselves in the merchant's shoes. It is meant to
          partner on the long run, and work as an extension of the merchant's
          team.`"
    />
  </div>
</template>

<script>
import P_Menu from "../organisms/P_Menu.vue";
import P_Hero_image from "../molecules/P_Hero_image.vue";

export default {
  components: {
    P_Menu,
    P_Hero_image,
  },
};
</script>

<style lang="scss"></style>
