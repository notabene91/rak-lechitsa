<template>
  <section class="about bg_violet">
    <!-- Размер теста в этом заголовке отличен от глобальных -->
    <h1 class="about__caption caption caption_h1">#РАКЛЕЧИТСЯ</h1>

    <!-- Обёртка контента для паддингов -->
    <div class="about__content">
      <h2 class="about__heading caption caption_h2">О проекте</h2>

      <div class="about__columns">
        <p class="about__desc paragraph">
          Этот проект был создан благотворительным фондом Константина
          Хабенского.
        </p>

        <div class="about__maintext">
          <div class="about__subjects">
            <p
              class="about__subject about__subject_active paragraph"
              @click="toggleSubject"
            >
              Рак Лечится
            </p>
            <p class="about__subject paragraph" @click="toggleSubject">
              Фонд Хабенского
            </p>
          </div>
          <div class="paragraphs" v-html="cancer" v-if="isShow"></div>
          <div class="paragraphs" v-html="fond" v-if="!isShow"></div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  methods: {
    toggleSubject() {
      if (event.target.classList.contains('about__subject_active')) {
        event.target.classList.add('about__subject_active');
      } else {
        event.target.classList.toggle('about__subject_active');
      }
      this.isShow = !this.isShow;
    },
  },
  data() {
    return {
      isShow: true,
      cancer:
        '<p class="about__paragraph paragraph" style="margin: 0"> Есть вещи, которые не лечатся. Особенности характера, страстные увлечения, привычки, ставшие частью нашего «я», фобии, которые мы приобрели в детстве. Список можно продолжать до бесконечности, но одна болезнь в него точно не войдет. Эта болезнь — рак. Рак лечится, и лучшее доказательство — люди с их неизлечимыми особенностями, которые сумели победить рак.</p><p class="about__paragraph paragraph"> Рак лечится — проект Благотворительного Фонда Константина Хабенского и Leo Burnett Moscow. С его помощью мы надеемся изменить отношение людей к раку и заставить каждого поверить: онкологическое заболевание — это не приговор.</>',
      fond:
        '<p class="about__paragraph paragraph" style="margin: 0">Благотворительный Фонд Константина Хабенского с 2008 года помогает детям с онкологическими и другими тяжелыми заболеваниями головного мозга. Фонд не только поддерживает семью заболевшего ребенка в самый сложный момент, оплачивая обследования, лечение и медицинские препараты, но и в целом меняет систему оказания помощи детям с опухолями мозга в России.</p>',
    };
  },
};
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
.about__subjects {
  margin-right: 40px;
  cursor: pointer;
  color: #c9c9c9;
}

.about__subject_active {
  font-weight: 500;
  color: #ffffff;
}

.about__subject {
  text-align: right;
  margin: 0 0 10px;
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
