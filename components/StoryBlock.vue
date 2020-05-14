<template>
  <section class="storyblock">
    <h2 class="storyblock__caption caption caption_h2">
      Истории неизлечимых привычек
    </h2>
    <div class="storyblock__grid">
      <storyGrid />
    </div>
    <div class="storyblock__button">
      <button class="storyblock__button large-btn">Больше статей</button>
    </div>
  </section>
</template>

<script>
import StoryGrid from '@/components/StoryGrid';
export default {
  components: {
    storyGrid: StoryGrid,
  },
};
</script>

<style scoped>
.storyblock__caption {
  max-width: 420px;
  margin-bottom: 70px;
  text-align: left;
}
.storyblock__button {
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
  .storyblock__caption {
    padding: 90px 0 60px;
  }
  .storyblock__button {
    height: 78px;
  }
}

@media (max-width: 1024px) {
  .storyblock__caption {
    max-width: 288px;
    font-size: 24px;
    line-height: 28px;
    padding: 80px 0 46px;
  }

  .storyblock__button {
    height: 50px;
    font-size: 13px;
  }
}

@media (max-width: 768px) {
  .storyblock__caption {
    font-size: 24px;
    line-height: 28px;
    padding: 80px 0 60px;
    text-align: center;
    margin: 0 auto;
  }
}

@media (max-width: 320px) {
  .storyblock__caption {
    font-size: 18px;
    line-height: 21px;
    padding: 50px 0 40px;
    text-align: left;
  }
  .storyblock__button {
    margin-top: 10px;
  }
}
</style>
