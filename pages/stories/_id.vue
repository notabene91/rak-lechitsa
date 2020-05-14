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

<style scoped>
.id /* deep */ .active,
.id /* deep */ .active:visited,
.id /* deep */ .active:hover {
  text-decoration: none;
}
</style>
