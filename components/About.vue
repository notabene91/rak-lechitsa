<template>
  <section class="about bg_violet">
    <!-- Размер теста в этом заголовке отличен от глобальных -->
    <h1 class="about__caption caption caption_h1">
      #РАКЛЕЧИТСЯ
    </h1>

    <!-- Обёртка контента для паддингов -->
    <div class="about__content container">
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
  width: 100%;
  padding: 0 0 100px 0;
  margin: 0 auto;
}

.about__heading {
  color: #fff;
  margin-bottom: 32px;
  text-align: left;
}

.about__desc {
  color: #dedede;
  max-width: 340px;
  margin: 0;
}

.about__columns,
.about__maintext {
  display: flex;
  justify-content: space-between;
}
.about__subject {
  margin-right: 40px;
}

.about__fond-name {
  text-align: right;
  color: #c9c9c9;
  margin: 0 0 10px 0;
}
.about__fond-founder {
  text-align: right;
  color: #c9c9c9;
  margin: 0;
}

/* Навесить на активную надпись */
.about__fond_ative {
  font-weight: 500;
  color: #fff;
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

@media (max-width: 1280px) {
  .about__content {
    padding: 0 0 90px 0;
  }
  .about__caption {
    margin-bottom: 60px;
    padding-top: 80px;
    font-size: 58px;
    line-height: 70px;
  }

  .about__heading {
    margin-bottom: 30px;
    text-align: left;
  }

  .about__desc {
    max-width: 305px;
    margin: 0;
    font-size: 16px;
    line-height: 20px;
  }

  .paragraphs {
    max-width: 570px;
  }
}

@media (max-width: 1024px) {
  .about__content {
    padding: 0 0 80px 0;
  }
  .about__caption {
    margin-bottom: 60px;
    padding-top: 80px;
    font-size: 52px;
    line-height: 63px;
  }

  .about__heading {
    margin-bottom: 30px;
    text-align: left;
  }

  .about__desc {
    max-width: 260px;
    margin: 0;
    font-size: 13px;
    line-height: 16px;
  }

  .about__fond-name {
    font-size: 15px;
    line-height: 19px;
    margin: 0 0 8px 0;
  }

  .about__fond-founder {
    font-size: 15px;
    line-height: 19px;
  }

  .paragraphs {
    max-width: 450px;
  }

  .about__paragraph {
    font-size: 15px;
    line-height: 19px;
  }
}

@media (max-width: 768px) {
  .about__content {
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 80px 0 80px 0;
  }

  .about__columns,
  .about__maintext {
    flex-direction: column;
    align-items: flex-start;
    margin: 0 auto;
  }

  .about__heading {
    margin-bottom: 26px;
    text-align: center;
  }

  .about__desc {
    max-width: 380px;
    margin: 0 0 80px 0;
    font-size: 13px;
    line-height: 16px;
  }

  .about__subject {
    margin-bottom: 30px;
    display: flex;
    align-content: flex-start;
  }

  .about__fond-name {
    font-size: 15px;
    line-height: 19px;
    margin: 0 30px 0 0;
  }

  .about__fond-founder {
    font-size: 15px;
    line-height: 19px;
  }

  .about__fond_ative {
    font-weight: 500;
    color: #fff;
    border-bottom: 2px solid #fff;
  }

  .paragraphs {
    max-width: 380px;
  }
  .about__caption {
    display: none;
  }
}

@media (max-width: 320px) {
  .about__content {
    padding: 50px 0 50px 0;
  }

  .about__heading {
    margin: 0 0 16px 0;
    text-align: left;
  }

  .about__desc {
    max-width: 290px;
    margin: 0 0 40px 0;
  }

  .about__subject {
    margin-bottom: 20px;
  }

  .about__fond-name {
    font-size: 13px;

    margin: 0 16px 0 0;
  }

  .about__fond-founder {
    font-size: 13px;
  }

  .paragraphs {
    max-width: 290px;
  }
}
</style>
