<template>
  <div class="id">
    <StoryTitle />
    <StoryText />
  </div>
</template>

<script>
import StoryTitle from '@/components/StoryTitle';
import StoryText from '@/components/StoryText';
export default {
  components: {
    StoryTitle: StoryTitle,
    StoryText: StoryText,
  },
};
</script>

<style scoped></style>
