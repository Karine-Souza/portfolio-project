<template>
  <div class="image">
    <img
      :src="src"
      :alt="alt"
      :class="aditionalClass"
      :href="href"
      :width="width"
      :height="height"
    />
  </div>
</template>

<script>
export default {
  props: {
    src: {
      type: String,
    },
    alt: {
      type: String,
    },
    aditionalClass: {
      type: String,
    },
    href: {
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
.image {
  margin: 0;
  padding: 0;
}
</style>
