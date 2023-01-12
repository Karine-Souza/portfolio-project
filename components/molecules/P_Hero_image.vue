<template>
  <div class="heroImage">
    <div class="heroImage__container">
      <div class="heroImage__textSide">
        <a class="heroImage__link" href="#">About</a>
        <h1 class="heroImage__title">An Experience Design Agency</h1>
        <h5 class="heroImage__subtitle">Provides a full service range</h5>
        <p class="heroImage__texto">
          Ability to put themselves in the merchant's shoes. It is meant to
          partner on the long run, and work as an extension of the merchant's
          team.
        </p>
        <P_Button
          class="heroImage__button"
          :label="'About Us'"
          :backgroundColor="'#Ffffff'"
          :width="''"
          :height="''"
        />
      </div>
      <div class="heroImage__imageSide">
        <P_Image class="image" :src="require('@/assets/images/Bitmap8.png')" />
      </div>
    </div>
  </div>
</template>

<script>
import P_Button from "../atoms/P_Button.vue";
import P_Image from "../atoms/P_Image.vue";

export default {
  components: {
    P_Button,
    P_Image,
  },
};
</script>

<style lang="scss">
.heroImage {
  width: 100%;
  height: 880px;
  align-items: center;
  justify-content: center;
  background-color: #fdf0e9;
  display: flex;
  @media (min-width: 992px) {
  }
  @media (min-width: 1280px) {
  }
  &__container {
    flex-direction: column-reverse;
    display: flex;
    padding: 60px;
    @media (min-width: 992px) {
      flex-direction: column-reverse;
    }
    @media (min-width: 1280px) {
      flex-direction: row-reverse;
    }
  }

  &__imageSide {
    display: flex;
    align-items: center;
    justify-content: center;
    @media (min-width: 992px) {
      image {
        width: 566px;
        height: 585px;
      }
    }
    @media (min-width: 1280px) {
      image {
        width: 566px;
        height: 585px;
      }
    }
  }
  &__textSide {
    margin: 15px;

    @media (min-width: 992px) {
    }
    @media (min-width: 1280px) {
      margin: 171px 188px 240px 130px;
    }
  }

  &__link {
    text-decoration: none;
    color: #ef6d58;
  }
  &__title {
  }
  &__subtitle {
  }
  &__text {
  }
}
</style>
