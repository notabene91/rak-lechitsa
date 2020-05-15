<template>
  <div class="id">
    <StoryTitle />
    <StoryText />
    <div class="id__grid">
      <storyGrid />
    </div>
    <div class="id__button">
      <button class="id__button large-btn">Больше историй</button>
    </div>
  </div>
</template>

<script>
import StoryTitle from '@/components/StoryTitle';
import StoryText from '@/components/StoryText';
import StoryGrid from '@/components/StoryGrid';
export default {
  components: {
    StoryTitle: StoryTitle,
    StoryText: StoryText,
    storyGrid: StoryGrid,
  },
};
</script>

<style scoped>
.id__grid {
  margin-top: 50px;
}
.id__button {
  max-width: 100%;
  height: 82px;
  padding: 0;
  border: none;
  font-family: 'Inter', sans-serif;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 20px;
}

@media (max-width: 1280px) {
  .id__button {
    height: 78px;
  }
}

@media (max-width: 1024px) {
  .id__button {
    height: 50px;
    font-size: 13px;
  }
}

@media (max-width: 320px) {
  .id__button {
    margin-top: 10px;
  }
}
</style>
