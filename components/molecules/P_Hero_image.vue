<template>
  <div class="heroImage">
    <div
      class="heroImage-container"
      :style="{
        backgroundColor: '#EDF3FF',
      }"
    ></div>
  </div>
</template>

<script>
export default {
  components: {},
};
</script>

<style lang="scss">
.heroImage {
  width: 100%;
  height: 880px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 73px 0 0;
  .heroImage__container {
    display: flex;
    flex-direction: row-reverse;
    padding: 60px;
  }
}
</style>
