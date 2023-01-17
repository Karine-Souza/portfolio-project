<template>
  <div class="latestWork" :style="{ background: backgroundColor }">
    <P_Card
      :src="require('@/assets/images/pic (3).png')"
      :categoria="designer"
    />
  </div>
</template>

<script>
import P_Card from "../molecules/P_Card";

export default {
  components: {
    P_Card,
  },
};
</script>

<style lang="scss"></style>
