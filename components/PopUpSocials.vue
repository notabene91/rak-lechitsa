<template>
  <div class="popup-socials">
    <img src="/img/cross.svg" alt="" class="popup__close" />
    <h2 class="popup__stage">Поделитесь</h2>

    <div class="popup-socials-links">
      <a href="#" class=" link popup__link" target="_blank">
        <img
          class="popup-socials-icon"
          src="/img/socials/Facebook.svg"
          alt="иконка  - перейти на Facebook"
      /></a>
      <a href="#" class=" link popup__link" target="_blank">
        <img
          class="popup-socials-icon"
          src="/img/socials/Twitter.svg"
          alt="иконка  - перейти на Twitter"
      /></a>
      <a href="#" class=" link popup__link" target="_blank">
        <img
          class="popup-socials-icon"
          src="/img/socials/Vkontakte.svg"
          alt="иконка  - перейти на Vkontakte"
      /></a>
      <a href="#" class=" link popup__link" target="_blank">
        <img
          class="popup-socials-icon"
          src="/img/socials/Odnoklassniki.svg"
          alt="иконка  - перейти на Odnoklassniki"
      /></a>
      <a href="#" class=" link popup__link" target="_blank">
        <img
          class="popup-socials-icon"
          src="/img/socials/Instagram.svg"
          alt="иконка  - перейти на Instagram"
      /></a>
      <a href="#" class=" link popup__link" target="_blank">
        <img
          class="popup-socials-icon"
          src="/img/socials/YouTube.svg"
          alt="иконка  - перейти на YouTube"
      /></a>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.popup-socials {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 63.89%;
  max-width: 920px;
  min-height: 324px;
  box-sizing: border-box;
  padding: 40px;
  background-color: #fff;
  z-index: 2;
}
.popup__stage {
  padding-bottom: 100px;
  margin: 0 auto;
  text-align: center;
  font-weight: 600;
  font-size: 32px;
  line-height: 36px;
}

.popup-socials-links {
  display: flex;
  justify-content: space-between;
  margin: 0 auto;
  padding-bottom: 60px;
}
.popup__close {
  position: absolute;
  top: 35px;
  right: 35px;
  cursor: pointer;
}

.popup__link {
  cursor: pointer;
  margin-right: 20px;
}

.popup__link:last-of-type {
  margin-right: 0px;
}

@media (max-width: 1280px) {
  .popup-socials {
    width: 62.5%;
    max-width: 800px;
  }
}

@media (max-width: 1024px) {
  .popup-socials {
    width: 78.13%;
    max-width: 800px;
  }
}

@media (max-width: 768px) {
  .popup-socials {
    width: 75.52%;
    max-width: 580px;
  }
}

@media (max-width: 320px) {
  .popup-socials {
    width: 90.63%;
    max-width: 290px;
    min-height: 191px;
    padding: 15px 0 0;
  }
  .popup__stage {
    padding-bottom: 60px;

    font-weight: 600;
    font-size: 18px;
    line-height: 21px;
  }

  .popup__close {
    top: 13px;
    right: 11px;
  }

  .popup__link {
    cursor: pointer;
    margin-right: 14px;
  }
  .popup-socials-icon {
    width: 35px;
  }
}
</style>
