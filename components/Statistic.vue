<template>
  <section class="statistic container">
    <h2 class="statistic__title">Статистика по онкозаболеваниям</h2>
    <div class="statistic__container">
      <statistic-card
        v-for="card in cards"
        :key="card.id"
        :info="card.info"
        :numbers="card.numbers"
        :source="card.source"
      ></statistic-card>
    </div>
  </section>
</template>

<script>
import StatisticCard from '@/components/Statistic-card';
export default {
  components: {
    'statistic-card': StatisticCard,
  },
  data() {
    return {
      cards: [
        {
          id: '1',
          info:
            'Каждый 3-й в стране уверен, что рак неизлечим. А это примерно 48 918 000 человек.',
          numbers: '1 из 3',
          source: 'Левада-Центр 2018',
        },
        {
          id: '2',
          info: '2,6% Россиян имеют онкозаболевания.',
          numbers: '3 700 000',
          source: 'Росстат 2018',
        },
        {
          id: '3',
          info:
            'На 28% выросла доля выявления заболеваний на ранней стадии за 10 лет.',
          numbers: '↑28%',
          source: 'МНИОИ Герцена 2018',
        },
        {
          id: '4',
          info:
            'На 25% снизилась смертность в течение первого года после постановки диагноза.',
          numbers: '↓25%',
          source: 'МНИОИ Герцена 2018',
        },
      ],
    };
  },
};
</script>

<style scoped>
.statistic {
  margin: 0 auto;
}

.statistic__title {
  max-width: 340px;
  margin: 0 0 90px 0;
  font-size: 32px;
  line-height: 36px;
}

.statistic__container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
</style>
