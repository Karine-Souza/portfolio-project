<template>
  <div class="card" :src="src">
    <div class="card__content">
      <P_Tag_button :label="label" :href="href" />
      <h1 class="card__categororia">{{ categoria }}</h1>
    </div>
  </div>
</template>

<script>
import P_Tag_button from "../atoms/P_Tag_button.vue";

export default {
  components: {
    P_Tag_button,
  },
  props: {
    src: {
      type: String,
    },
    label: {
      type: String,
    },
    href: {
      type: String,
    },
    categoria: {
      type: String,
    },
    aditionalClasses: {
      type: String,
    },
  },
};
</script>

<style lang="scss">
.card {
  position: absolute;
  width: 370px;
  height: 416px;
  opacity: 0.32;
  border-radius: 6px;
  background: #5c2000;
  mix-blend-mode: normal;
  color: #ffffff;
}
</style>
