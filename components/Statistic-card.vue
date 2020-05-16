<template>
  <div class="statistic-card">
    <p class="statistic-card__info">{{ info }}</p>

    <div class="statistic-card__container">
      <progress-bar
        :currentBarValue="currentBarValue"
        :maxBarValue="maxBarValue"
        :oldBarValue="oldBarValue"
      ></progress-bar>
      <p class="statistic-card__numbers">{{ numbers }}</p>
      <p class="statistic-card__source">{{ source }}</p>
    </div>
  </div>
</template>

<script>
import ProgressBar from '@/components/ui/ProgressBar';
export default {
  components: {
    'progress-bar': ProgressBar,
  },
  props: [
    'info',
    'numbers',
    'source',
    'currentBarValue',
    'maxBarValue',
    'oldBarValue',
  ],
};
</script>

<style scoped>
.statistic-card {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  width: 300px;
  height: 300px;
  padding: 20px;
  box-sizing: border-box;
}

.statistic-card:nth-of-type(4n) {
  margin-right: 0;
}

.statistic-card__info {
  font-size: 12px;
  line-height: 16px;
  margin: 0;
  color: #000;
}

.statistic-card__progress {
  background-color: #613a93;
  height: 40px;
  margin-bottom: 20px;
}

.statistic-card__numbers {
  font-size: 38px;
  line-height: 40px;
  font-weight: 600;
  color: #000;
  margin: 0 0 20px;
  text-align: right;
}

.statistic-card__source {
  font-size: 12px;
  line-height: 16px;
  color: #666;
  margin: 0;
  text-align: right;
}
</style>
