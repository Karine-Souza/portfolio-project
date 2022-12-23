<template>
  <div class="footer">
    <div class="footer__nav">
      <div class="footer__logo">
        <img src="../../assets/images/Webflow_logo.png" />
      </div>
      <div class="footer__menu">
        <ul class="footer__navListMenu">
          <li>
            <h5 class="footer__navItem1">MENU</h5>
          </li>
          <li>
            <a class="footer__navItem2" href="#" target="_blank">About</a>
          </li>
          <li>
            <a class="footer__navItem3" href="#" target="_blank">Services</a>
          </li>
          <li>
            <a class="footer__navItem4" href="#" target="_blank">Blog</a>
          </li>
          <li>
            <a class="footer__navItem5" href="#" target="_blank">Contact</a>
          </li>
        </ul>
      </div>
      <div class="footer__service">
        <ul class="footer__navListService">
          <li>
            <h5 class="footer__navItem1">SERVICE</h5>
          </li>
          <li>
            <a class="footer__navItem1" href="#" target="_blank">Design</a>
          </li>
          <li>
            <a class="footer__navItem2" href="#" target="_blank">Development</a>
          </li>
          <li>
            <a class="footer__navItem3" href="#" target="_blank">Marketing</a>
          </li>
          <li>
            <a class="footer__navItem3" href="#" target="_blank">See More</a>
          </li>
        </ul>
      </div>
      <P_Social_media />
    </div>
    <div class="footer__line"></div>
    <div class="footer__copyMenu">
      <div class="footer__copyText">
        <p>Copyright © 2022 Laaqiq. All Rights Reserved.</p>
      </div>
      <div class="footer__copyLinks">
        <ul class="footer__copyList">
          <li>
            <a class="footer__copyItem1" href="#" target="_blank"
              >Terms of Use</a
            >
          </li>
          <li>
            <a class="footer__copyItem2" href="#" target="_blank"
              >Privacy Policy</a
            >
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import P_Social_media from "../../components/molecules/P_Social_media";

export default {
  components: {
    P_Social_media,
  },
};
</script>

<style lang="scss">
.footer {
  width: 100%;
  background-color: #fdf0e9;
  color: #000000;

  @media (min-width: 992px) {
  }
  @media (min-width: 1280px) {
  }

  &__nav {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
    @media (min-width: 992px) {
    }
    @media (min-width: 1280px) {
      padding: 217px 135px 68px 135px;
      flex-direction: row;
      align-items: flex-start;
      justify-content: space-between;
    }
    .socialMedia {
      margin: 52px 0 65px 0;
      @media (min-width: 992px) {
      }
      @media (min-width: 1280px) {
        margin: 15px 0 0 0;
      }
    }
  }

  &__logo {
    position: relative;
    margin-top: 15px;
    img {
      width: 106px;
    }
  }

  &__menu {
    margin: 0;
    padding: 0;
  }

  &__navListMenu {
    list-style: none;
    margin: 0;
    padding: 0;
    a {
      text-decoration: none;
      color: #000000;
      font: normal normal 400 16px/32px "Epilogue";
    }
    li:first-child {
      color: #ef6d58;
      text-decoration: none;
      list-style: none;
      font: normal normal 400 16px/32px "Epilogue";
      letter-spacing: 3px;
    }
  }

  &__navListService {
    list-style: none;
    margin: 0;
    padding: 0;
    a {
      text-decoration: none;
      color: #000000;
      font: normal normal 400 16px/32px "Epilogue";
    }
    li:first-child {
      color: #ef6d58;
      text-decoration: none;
      list-style: none;
      font: normal normal 400 16px/32px "Epilogue";
      letter-spacing: 3px;
    }
  }

  &__line {
    position: absolute;
    width: 100%;
    border-bottom: 1px solid #ef6d58;
    opacity: 0.5;

    @media (min-width: 992px) {
    }
    @media (min-width: 1280px) {
    }
  }

  &__copyMenu {
    display: flex;
    flex-direction: column;
    padding: 43px 88px;
    align-items: center;
    justify-content: space-between;
    @media (min-width: 992px) {
    }
    @media (min-width: 1280px) {
      flex-direction: row;
      padding: 43px 135px;
    }
  }

  &__copyText {
    color: #000000;
    font: normal normal 400 16px/32px "Epilogue";
    letter-spacing: 0px;
    text-align: center;
    display: flex;
    @media (min-width: 1280px) {
      text-align: left;
    }
  }

  &__copyLinks {
    width: 275px;
    a {
      text-decoration: none;
      color: black;
    }
  }

  &__copyList {
    display: flex;
    font: normal normal 400 16px/32px "Epilogue";
    list-style: none;
    justify-content: space-between;
    padding: 0;
  }
}
</style>
