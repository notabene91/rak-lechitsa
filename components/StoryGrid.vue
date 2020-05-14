<template>
  <section class="story-grid">
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

@media (max-width: 1280px) {
  .story-grid__item {
    margin-bottom: 60px;
  }
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
