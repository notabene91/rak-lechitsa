<template>
  <section class="story-grid container">
    <h2 class="story-grid__caption caption caption_h2">
      Истории неизлечимых привычек
    </h2>
    <div class="story-grid__container">
      <div class="story-grid__item"><storyCard /></div>
      <div class="story-grid__item"><storyCard /></div>
      <div class="story-grid__item"><storyCard /></div>
      <div class="story-grid__item"><storyCard /></div>
      <div class="story-grid__item"><storyCard /></div>
      <div class="story-grid__item"><storyCard /></div>
      <div class="story-grid__item"><storyCard /></div>
      <div class="story-grid__item"><storyCard /></div>
    </div>

    <button class="story-grid__button large-btn">Больше статей</button>
  </section>
</template>

<script>
import StoryCard from '@/components/StoryCard';
export default {
  components: {
    storyCard: StoryCard,
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

.story-grid__caption {
  max-width: 420px;
  padding: 100px 0 70px;
  text-align: left;
}

.story-grid__container {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}

.story-grid__item {
  margin-bottom: 70px;
  max-width: fit-content;
  width: 100%;
}

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

@media (max-width: 1280px) {
  .story-grid__caption {
    padding: 90px 0 60px;
  }

  .story-grid__item {
    margin-bottom: 60px;
  }
  .story-grid__button {
    height: 78px;
  }
}

@media (max-width: 1024px) {
  .story-grid__caption {
    max-width: 288px;
    font-size: 24px;
    line-height: 28px;
    padding: 80px 0 46px;
  }

  .story-grid__item {
    margin-bottom: 46px;
  }
  .story-grid__button {
    height: 50px;
    font-size: 13px;
  }
}

@media (max-width: 768px) {
  .story-grid__caption {
    font-size: 24px;
    line-height: 28px;
    padding: 80px 0 60px;
    text-align: center;
    margin: 0 auto;
  }

  .story-grid__item {
    margin-bottom: 56px;
  }
}

@media (max-width: 320px) {
  .story-grid__caption {
    font-size: 18px;
    line-height: 21px;
    padding: 50px 0 40px;
    text-align: left;
  }

  .story-grid__item {
    margin-bottom: 30px;
  }
  .story-grid__button {
    margin-top: 10px;
  }
}
</style>
