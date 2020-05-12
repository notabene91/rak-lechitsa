<template>
  <section class="tell container">
    <h2 class="tell__title">Расскажите свою историю</h2>
    <div class="tell__container">
      <p class="tell__text">
        Мы публикуем новые истории на сайте раз в неделю. Есть 2 варианта
        поделиться своей историей неизлечимых привычек, навязчивых идей и
        болезненных привязанностей.
      </p>

      <div class="tell__variants">
        <p class="tell__variant tell__variant_active">1-й вариант</p>
        <p class="tell__variant">2-й вариант</p>
      </div>

      <div class="tell__instruction">
        <p class="tell__instruction-text">
          Заполнить подробную форму прямо на сайте и мы опубликуем вашу историю
          после проверки. Пожалуйста, заполняйте все пункты корректно, если вы
          испытаете какие-то сложности, воспользуйтесь 2-м вариантом.
        </p>
        <button class="btn tell__btn">Заполнить форму</button>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
.tell {
  margin: 0 auto;
  background-color: #f7f7f7;
}

.tell__container {
  display: flex;
  justify-content: space-between;
}

.tell__title {
  margin: 0 0 32px 0;
  max-width: 340px;
  font-size: 32px;
  line-height: 36px;
}

.tell__text {
  margin: 0 192px 0 0;
  max-width: 340px;
  color: #666;
  line-height: 22px;
}

.tell__variant {
  margin: 0 0 10px;
  color: #a2a2a2;
}

.tell__variant_active {
  color: #000;
}

.tell__instruction {
  max-width: 640px;
  margin-left: 40px;
}

.tell__instruction-text {
  margin: 0 0 72px;
  color: #666;
}
</style>
