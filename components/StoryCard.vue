<template>
  <section class="story-card">
    <!-- Ни разу не пользовался тего пикча
    Не уверен, что правильно сделал.
    Картинки пока не клал в проект-->
    <picture class="story-card__picture">
      <source
        srcset="http://ipic.su/img/img7/fs/Tan.1589128962.jpg"
        media="(min-width: 1440px)"
      />
      <source
        srcset="http://ipic.su/img/img7/fs/Tan265.1589129491.jpg"
        media="(max-width: 1280px)"
      />
      <img src="#" alt="фотография автора цитаты" />
    </picture>
    <cite class="story-card__author">
      Владимир Тен
    </cite>
    <blockquote class="story-card__quote">
      Я всегда читаю книги с конца, - и это не лечится, в отличие от рака.
    </blockquote>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
.story-card {
  display: flex;
  flex-direction: column;
}

.story-card__picture {
  max-width: 300px;
  max-height: 300px;
  margin-bottom: 20px;
}
.story-card__author {
  font-style: normal;
  font-weight: 600;
  font-size: 22px;
  line-height: 22px;
  color: #000000;
  margin-bottom: 14px;
}
.story-card__quote {
  max-width: 250px;
  font-size: 14px;
  line-height: 18px;
  color: #666666;
  padding: 0;
  margin: 0;
}
</style>
