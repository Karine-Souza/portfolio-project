<template>
  <div class="header">
    <P_Menu />
    <P_Hero_image />
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
