<template>
  <section class="about bg_violet">
    <!-- Размер теста в этом заголовке отличен от глобальных -->
    <h1 class="about__caption caption caption_h1">
      #РАКЛЕЧИТСЯ
    </h1>

    <!-- Обёртка контента для паддингов -->
    <div class="about__content">
      <h2 class="about__heading caption caption_h2">
        О проекте
      </h2>

      <div class="about__columns">
        <p class="about__desc paragraph">
          Этот проект был создан благотворительным фондом Константина
          Хабенского.
        </p>

        <div class="about__maintext">
          <div class="about__subject">
            <p class="about__fond-name paragraph">Рак Лечится</p>
            <p class="about__fond-founder paragraph">Фонд Хабенского</p>
          </div>
          <div class="paragraphs">
            <p class="about__paragraph paragraph">
              Есть вещи, которые не лечатся. Особенности характера, страстные
              увлечения, привычки, ставшие частью нашего «я», фобии, которые мы
              приобрели в детстве. Список можно продолжать до бесконечности, но
              одна болезнь в него точно не войдет. Эта болезнь — рак. Рак
              лечится, и лучшее доказательство — люди с их неизлечимыми
              особенностями, которые сумели победить рак.
            </p>
            <p class="about__paragraph paragraph">
              Рак лечится — проект Благотворительного Фонда Константина
              Хабенского и Leo Burnett Moscow. С его помощью мы надеемся
              изменить отношение людей к раку и заставить каждого поверить:
              онкологическое заболевание — это не приговор.
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
.about {
  display: flex;
  flex-direction: column;
}
/* Размер теста в этом заголовке отличен от глобальных */
.about__caption {
  margin-bottom: 70px;
  padding-top: 90px;
  text-align: center;
  font-weight: 800;
  font-size: 64px;
  line-height: 77px;
}

.about__content {
  padding: 0 60px 100px 60px;
}

.about__heading {
  color: #ffffff;
  margin-bottom: 32px;
  text-align: left;
}

.about__desc {
  color: #dedede;
  max-width: 340px;
  margin: 0;
}

.about__columns {
  display: flex;
  justify-content: space-between;
}

.about__maintext {
  display: flex;
  justify-content: space-between;
}
.about__subject {
  margin-right: 40px;
}
.about__fond-name {
  text-align: right;
  font-weight: 500;
  color: #ffffff;
  margin: 0 0 10px 0;
}
.about__fond-founder {
  text-align: right;
  color: #c9c9c9;
  margin: 0;
}
.paragraphs {
  max-width: 640px;
  color: #dedede;
}
.about__paragraph {
  margin: 0 0 20px 0;
}
.about__paragraph:last-of-type {
  margin: 0;
}
</style>
