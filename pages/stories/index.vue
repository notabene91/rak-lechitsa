<template>
  <div class="stories">
    <div class="container stories__container">
      <div class="stories__item">
        <search />
      </div>
      <div class="stories__item">
        <!-- тут будет дата для количества -->
        <!-- тут надо будет переделать: убрать заголовок из количества -->
        <storyGrid />
        <!-- блок ниже не сделан, его надо сделать и брать из UI -->
        <div class="story__buttons">
          <button class="story__button story__button_active">
            1
          </button>
          <button class="story__button">
            2
          </button>
          <button class="story__button">
            3
          </button>
          <button class="story__button">
            4
          </button>
          <button class="story__button">
            5
          </button>
          <button class="story__button">
            6
          </button>
          <button class="story__button">
            7
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Search from '@/components/Search';
import StoryGrid from '@/components/StoryGrid';
export default {
  components: {
    search: Search,
    storyGrid: StoryGrid,
  },
};
</script>

<style>
.stories__container {
  margin: 0 auto;
}
.story__buttons {
  padding-bottom: 40px;
  max-width: fit-content;
  /* убрать отступ сверху */
  margin: 10px auto 0;
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
/* из-за временного скрытия поехали стили */
.stories /* deep */ .story-grid__container {
  padding-top: 100px;
}
</style>
