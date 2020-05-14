<template>
  <section class="story-grid">
    <div class="story-grid__container">
      <storyCard
        class="story-grid__item"
        v-for="card in cards"
        :key="card.id"
        :author="card.author"
        :quote="card.quote"
        :picture="card.picture"
      />
    </div>
  </section>
</template>

<script>
import StoryCard from '@/components/StoryCard';
export default {
  components: {
    storyCard: StoryCard,
  },
  data() {
    return {
      cards: [
        {
          id: '1',
          picture: 'http://ipic.su/img/img7/fs/Tan.1589128962.jpg',
          author: 'Владимир Тен',
          quote:
            'Я всегда читаю книги с конца, - и это не лечится, в отличие от рака.',
        },
        {
          id: '2',
          picture: 'http://ipic.su/img/img7/fs/Tan.1589128962.jpg',
          author: 'Владимир Познер',
          quote: 'Я боюсь акул — и, в отличии от рака, это не лечится.',
        },
        {
          id: '3',
          picture: 'http://ipic.su/img/img7/fs/Tan.1589128962.jpg',
          author: 'Александр Тарханов',
          quote: 'Я не могу победить свою пунктуальность в отличии от рака.',
        },
        {
          id: '4',
          picture: 'http://ipic.su/img/img7/fs/Tan.1589128962.jpg',
          author: 'Владимир Тен',
          quote:
            'Я всегда читаю книги с конца, - и это не лечится, в отличие от рака.',
        },
      ],
    };
  },
};
</script>

<style scoped>
.story-grid {
  max-width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.story-grid__container {
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}

.story-grid__item {
  margin-bottom: 70px;
  max-width: fit-content;
  width: 100%;
}

<<<<<<< HEAD
.story-grid__button {
  max-width: 100%;
  height: 82px;
  padding: 0;
  border: none;
  font-family: Inter;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 20px;
}
.story__buttons {
  margin: 0 auto;
  padding-bottom: 40px;
  max-width: fit-content;
  /* убрать отступ сверху */
  margin: 10px auto 0;
}

=======
>>>>>>> caf3d2835a3cb17d1463a7d7ca2f9c7dc1c941ba
@media (max-width: 1280px) {
  .story-grid__item {
    margin-bottom: 60px;
  }
<<<<<<< HEAD
  .story-grid__button {
    height: 78px;
  }
  .story__button {
    width: 40px;
    height: 40px;
    background: #fbfbfb;
    border: none;
    padding: 0;
    margin-right: 10px;
    cursor: pointer;
  }
=======
>>>>>>> caf3d2835a3cb17d1463a7d7ca2f9c7dc1c941ba
}

@media (max-width: 1024px) {
  .story-grid__item {
    margin-bottom: 46px;
  }
}

@media (max-width: 768px) {
  .story-grid__item {
    margin-bottom: 56px;
  }
}

@media (max-width: 320px) {
  .story-grid__item {
    margin-bottom: 30px;
  }
}
</style>
