<template>
  <div class="cardTestimonials" :style="{ background: backgroundColor }">
    <div class="cardTestimonials__content">
      <img :src="srcStars" :alt="altStars" class="cardTestimonials__Stars" />
      <p class="cardTestimonials__Testimonials">{{ testimonials }}</p>
    </div>
    <div class="cardTestimonials__autor">
      <img
        :src="srcAutorImg"
        :alt="altAutorImg"
        class="cardTestimonials__Img"
      />
      <h5 class="cardTestimonials__nome">{{ nome }}</h5>
      <p class="cardTestimonials__profissão">{{ profissão }}</p>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  props: {
    backgroundColor: {
      type: String,
      default: "#FFFFFF",
    },
    srcStars: {
      type: String,
    },
    testimonials: {
      type: String,
    },
    srcAutorImg: {
      type: String,
    },
    nome: {
      type: String,
    },
    profissão: {
      type: String,
    },
  },
};
</script>

<style lang="scss">
.cardTestimonials {
  position: absolute;
  width: 586px;
  height: auto;
  border: 1px solid #f3d1bf;
}
</style>
