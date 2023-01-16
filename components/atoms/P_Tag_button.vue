<template>
  <a
    class="tagButton"
    :class="aditionalClasses"
    :href="href"
    target="_blank"
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
    func: {
      type: Function,
      default: () => {},
    },
    backgroundColor: {
      type: String,
      default: "#FFFFFF",
    },
  },
};
</script>

<style lang="scss">
.tagButton {
  position: relative;
  display: flex;
  width: 102px;
  height: 38px;
  border-radius: 19px;
  color: #391400;
  font: normal normal 400 16px/32px "Epilogue";
  text-align: center;
  align-items: center;
  justify-content: center;
  cursor: pointer;
}
</style>
