<template>
  <div
    class="heroImage"
    :style="{ background: backgroundColor }"
    :width="width"
    :height="height"
  >
    <div class="heroImage__container">
      <div class="heroImage__textSide">
        <a class="heroImage__link" :href="href">{{ link }}</a>
        <h1 class="heroImage__title">{{ titulo }}</h1>
        <h5 class="heroImage__subtitle">{{ subtitulo }}</h5>
        <p class="heroImage__text">{{ texto }}</p>
        <P_Button
          class="heroImage__button"
          :label="'About Us'"
          :backgroundColor="'#Ffffff'"
        />
      </div>
      <div class="heroImage__imageSide">
        <img class="heroImage__image" :src="src" :alt="alt" width="100%" />
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
  props: {
    label: {
      type: String,
    },
    src: {
      type: String,
    },
    alt: {
      type: String,
    },
    href: {
      type: String,
    },
    link: {
      type: String,
      required: true,
    },
    titulo: {
      type: String,
      required: true,
    },
    subtitulo: {
      type: String,
      required: true,
    },
    texto: {
      type: String,
      required: true,
    },
    backgroundColor: {
      type: String,
      default: "#FDF0E9",
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
.heroImage {
  width: 100%;
  height: auto;
  align-items: center;
  justify-content: center;
  background-color: #fdf0e9;
  display: flex;
  @media (min-width: 992px) {
    height: auto;
  }
  @media (min-width: 1280px) {
    height: auto;
  }
  &__container {
    flex-direction: column-reverse;
    display: flex;
    margin: 15px;
    @media (min-width: 992px) {
      flex-direction: column-reverse;
      margin: 65px;
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
      .heroImage__image {
        width: 55vw;
        height: 51.75vw;
        justify-content: center;
        align-items: center;
      }
    }
    @media (min-width: 1280px) {
      padding: 60px 65px 20px 20px;
      .heroImage__image {
        width: 42vw;
        height: 42vw;
      }
    }
  }
  &__textSide {
    @media (min-width: 992px) {
      justify-content: center;
      align-items: center;
    }
    @media (min-width: 1280px) {
      padding: 65px 20px 20px 60px;
    }
  }

  &__link {
    text-decoration: none;
    color: #ef6d58;
    @media (min-width: 992px) {
    }
    @media (min-width: 1280px) {
      font: normal normal 400 16px/32px "Epilogue";
    }
  }
  &__title {
    font: normal normal 800 40px/48px "Epilogue";
    @media (min-width: 992px) {
    }
    @media (min-width: 1280px) {
      width: 417px;
      font: normal normal 800 56px/64px "Epilogue";
    }
  }
  &__subtitle {
    font: normal normal 400 20px/32px "Epilogue";
    @media (min-width: 992px) {
    }
    @media (min-width: 1280px) {
      font: normal normal 400 20px/32px "Epilogue";
    }
  }
  &__text {
    color: #391400a3;
    font: normal normal 400 16px/32px "Epilogue";
    @media (min-width: 992px) {
    }
    @media (min-width: 1280px) {
      width: 470px;
      font: normal normal 400 16px/32px "Epilogue";
    }
  }
  &__button {
    @media (min-width: 992px) {
    }
    @media (min-width: 1280px) {
      font: normal normal 900 14px/14.35px "Epilogue";
    }
  }
}
</style>
