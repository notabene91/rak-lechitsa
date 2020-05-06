<template>
  <header class="header">
    <div class="header__container container">
      <div class="header__title strong">
        Проект благотворительного фонда<br />
        Константина Хабенского
      </div>
      <!-- это левый блок-->
      <nav class="header__nav">
        <!-- вот сюда будет подключаться главное меню, на место div's-->
        <div></div>
        <!-- вот на эту ссылку должен вешаться обработчик, который будет вызывать попап -->
        <span class="header__login">
          Рассказать историю
        </span>
      </nav>
    </div>
  </header>
</template>

<script>
export default {};
</script>

<style scoped>
.header {
  padding: 0 18px;
}
.header__container {
  margin: 0 auto;

  display: -webkit-flex;
  display: -webkit-box;
  display: -moz-flex;
  display: -moz-box;
  display: -ms-flexbox;
  display: -ms-flex;
  display: -o-flex;
  display: flex;
  -webkit-box-pack: justify;
  -webkit-justify-content: space-between;
  -ms-flex-pack: justify;
  justify-content: space-between;
  -webkit-box-align: center;
  -webkit-align-items: center;
  -ms-flex-align: center;
  align-items: center;
}
.header__login {
  cursor: pointer;
}
</style>
