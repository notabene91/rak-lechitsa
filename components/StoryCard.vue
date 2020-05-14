<template>
  <section class="story-card">
    <!-- Ни разу не пользовался тего пикча
    Не уверен, что правильно сделал.
    Картинки пока не клал в проект-->

    <picture class="story-card__picture">
      <img :src="picture" alt="фотография автора цитаты" />
    </picture>
    <cite class="story-card__author">
      {{ author }}
    </cite>
    <blockquote class="story-card__quote">
      {{ quote }}
    </blockquote>
  </section>
</template>

<script>
export default {
  props: ['picture', 'author', 'quote'],
};
</script>

<style scoped>
.story-card {
  display: flex;
  flex-direction: column;
}

.story-card__picture {
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

@media (max-width: 1024px) {
  .story-card__picture {
    margin-bottom: 16px;
  }
  .story-card__author {
    font-size: 18px;
  }
  .story-card__quote {
    max-width: 208px;
    font-size: 13px;
    line-height: 16px;
  }
}

@media (max-width: 768px) {
  .story-card__quote {
    max-width: 200px;
  }
}

@media (max-width: 320px) {
  .story-card__quote {
    max-width: 290px;
  }
}
</style>
