<template>
  <div>
    <Search />
    <StoryGrid />
  </div>
</template>

<script>
import Search from '@/components/search';
import StoryGrid from '@/components/StoryGrid';
export default {
  components: {
    Search: Search,
    StoryGrid: StoryGrid,
  },
};
</script>

<style></style>
