<template>
  <div class="popup">
    <div class="popup__container">
      <img src="/img/cross.svg" alt="" class="popup__close" />
      <h2 class="popup__stage">Шаг 1 из 12</h2>
      <p class="popup__question">
        <span class="popup__question_bold">Как вас зовут? </span>
      </p>
    </div>
    <div class="input__container">
      <input type="text" class="popup__input" placeholder="Напишите тут" />
      <a href="" class=" link popup__link">Назад</a>
      <button class=" btn popup__btn">Далее</button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.popup {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 60.5%;
  min-height: 600px;
  box-sizing: border-box;
  padding: 40px;
  background-color: #fff;
  z-index: 2;
}

.popup__close {
  position: absolute;
  top: 35px;
  right: 35px;
  cursor: pointer;
}

.popup__stage {
  margin: 0 0 40px;
  font-weight: 600;
  font-size: 32px;
  line-height: 36px;
}

.popup__question {
  font-weight: 400;
  font-size: 18px;
  line-height: 24px;
  margin: 0;
  color: #666;
}

.popup__question_bold {
  font-weight: 600;
  color: #000;
}

.popup__container {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.popup__input {
  width: 100%;
  margin-bottom: 200px;
  font-size: 18px;
  line-height: 24px;
  border: 0;
  border-bottom: 1px solid #e7e7e7;
}

.popup__btn {
  margin-left: 18px;
  padding: 16px 88px;
}

.popup__link {
  color: #c0c0c0;
  cursor: pointer;
}
</style>
