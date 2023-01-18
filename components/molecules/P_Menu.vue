<template>
  <div class="menu">
    <div class="menu_logo">
      <img src="../../assets/images/logo.png" class="footer_logoImg" />
    </div>
    <div class="menu__links">
      <ul class="menu__list">
        <li class="menu__listItems">
          <a class="menu__item menu__item1" href="#" target="_blank">About</a>
        </li>
        <li>
          <a class="menu__item menu__item2" href="#" target="_blank"
            >Services</a
          >
        </li>
        <li>
          <a class="menu__item menu__item3" href="#" target="_blank">Pricing</a>
        </li>
        <li>
          <a class="menu__item menu__item3" href="#" target="_blank">Blog</a>
        </li>
      </ul>
      <P_Button
        class="menu__button"
        label="Contact"
        :backgroundColor="'#28293e'"
      />
    </div>
  </div>
</template>

<script>
import P_Button from "../../components/atoms/P_Button.vue";

export default {
  components: {
    P_Button,
  },
};
</script>

<style lang="scss">
.menu {
  display: flex;
  background-color: #28293e;
  color: #ffffff;
  justify-content: space-between;
  align-items: center;
  padding: 14px 35px;

  @media (min-width: 992px) {
    padding: 14px 35px;
  }
  @media (min-width: 1280px) {
    padding: 14px 135px;
  }

  &__button {
    display: none;
    @media (min-width: 992px) {
      display: none;
    }
    @media (min-width: 1280px) {
      display: flex;
      width: 138px;
      border: 1px solid #707070;
    }
  }

  &__links {
    display: none;
    @media (min-width: 992px) {
      display: none;
    }
    @media (min-width: 1280px) {
      width: 75%;
      justify-content: space-between;
      display: flex;
    }
  }

  &__list {
    display: flex;
    list-style: none;
    justify-content: space-evenly;
    padding: 0;
    width: 80%;
  }

  &__item {
    text-decoration: none;
    color: #ffffff;
    font-family: "Epilogue", sans-serif;
  }
}
</style>
