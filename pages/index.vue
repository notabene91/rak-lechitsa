<template>
  <div class="index">
    <i-Banner />
    <div class="index__container container"></div>
  </div>
</template>

<script>
import Banner from '@/components/Banner';

export default {
  components: {
    'i-Banner': Banner,
  },
};
</script>

<style>
git .index__container {
  margin: 0 auto;
}
</style>
