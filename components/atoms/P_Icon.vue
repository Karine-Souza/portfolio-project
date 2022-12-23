<template>
  <div class="icon">
    <img
      :src="iconSrc"
      :alt="iconSrcAlt"
      class="section-icon"
      :class="iconAditionalClasses"
      :href="iconHref"
      :width="width"
      :height="height"
    />
  </div>
</template>

<script>
export default {
  props: {
    iconSrc: {
      type: String,
    },
    iconSrcAlt: {
      type: String,
    },
    iconAditionalClasses: {
      type: String,
    },
    iconHref: {
      type: String,
    },
    width: {
      type: String,
    },
    height: {
      type: String,
    },
  },
};
</script>

<style lang="scss">
.icon {
  margin: 0;
  padding: 0;
}
</style>
