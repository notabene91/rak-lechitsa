<template>
  <div class="index">
    <i-Banner />
    <div class="index__container container"></div>
  </div>
</template>

<script>
import Banner from '@/components/Banner';
import Statistic from '@/components/Statistic';
import Tell from '@/components/Tell';
import Overlay from '@/components/ui/Overlay';
import Popup from '@/components/PopUp';

export default {
  components: {
    'i-Banner': Banner,
    overlay: Overlay,
    popup: Popup,
    statistic: Statistic,
    tell: Tell,
  },
};
</script>

<style>
git .index__container {
  margin: 0 auto;
}
</style>
