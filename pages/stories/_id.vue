<template>
  <div class="id">
    <StoryTitle />
    <StoryText />
    <div class="id__grid">
      <storyGrid />
    </div>
    <div class="id__button">
      <bigGreyButton />
    </div>
  </div>
</template>

<script>
import StoryTitle from '@/components/StoryTitle';
import StoryText from '@/components/StoryText';
import StoryGrid from '@/components/StoryGrid';
import BigGreyButton from '@/components/ui/BigGreyButton';
export default {
  components: {
    StoryTitle: StoryTitle,
    StoryText: StoryText,
    storyGrid: StoryGrid,
    bigGreyButton: BigGreyButton,
  },
};
</script>

<style scoped>
.id__grid {
  margin-top: 50px;
}

/* @media (max-width: 1280px) {
  .
}

@media (max-width: 1024px) {

}

@media (max-width: 320px) {

} */
</style>
