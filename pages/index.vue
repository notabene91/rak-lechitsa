<template>
  <div class="index">
    <i-Banner />
    <div class="index__container container"></div>
    <tell />
    <statistic></statistic>
  </div>
</template>

<script>
import Banner from '@/components/Banner';
import Statistic from '@/components/Statistic';
import Tell from '@/components/Tell';
export default {
  components: {
    'i-Banner': Banner,
    statistic: Statistic,
    tell: Tell,
  },
};
</script>

<style>
.index__container {
  margin: 0 auto;
}
</style>
