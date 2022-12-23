<template>
  <a
    class="button"
    :class="aditionalClasses"
    :href="href"
    target="_blank"
    :width="width"
    :height="height"
    @click="func"
    :style="{ background: backgroundColor }"
    >{{ label }}</a
  >
</template>

<script>
export default {
  props: {
    href: {
      type: String,
    },
    label: {
      type: String,
      required: true,
    },
    aditionalClasses: {
      type: String,
    },
    width: {
      type: String,
    },
    height: {
      type: String,
    },
    func: {
      type: Function,
      default: () => {},
    },
    backgroundColor: {
      type: String,
      default: "#EF6D58",
    },
  },
};
</script>

<style lang="scss">
.button {
  position: relative;
  display: flex;
  width: 170px;
  height: 48px;
  border-radius: 7px;
  box-shadow: (0px 4px 4px rgba(0, 0, 0, 0.25));
  font: normal normal 900 14px/14px "Epilogue";
  text-align: center;
  text-transform: uppercase;
  align-items: center;
  justify-content: center;
  cursor: pointer;
}
</style>
