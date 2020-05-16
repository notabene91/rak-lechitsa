<template>
  <section class="instagram container">
    <div class="instagram__content">
      <div class="instagram__brief">
        <h2 class="instagram__caption caption caption_h2">Инстаграм</h2>
        <p class="instagram__desc">
          Два раза в неделю мы просматриваем все посты по хештегу #этонелечится.
          Все истории, где нет нецензурных выражений и запрещенного контента
          попадают сюда. Следите за правильным написанием хештега, чтобы мы не
          пропустили вашу историю.
        </p>
      </div>
      <div class="instagram__grid">
        <!-- тут надо править под vue -->
        <instagram-item
          class="instagram__grid-item"
          v-for="item in items"
          :key="item.id"
        ></instagram-item>
      </div>
    </div>
  </section>
</template>

<script>
import InstagramItem from '@/components/InstagramItem';
export default {
  components: {
    'instagram-item': InstagramItem,
  },
  data() {
    return {
      items: [
        {
          id: '1',
        },
        {
          id: '2',
        },
        {
          id: '3',
        },
        {
          id: '4',
        },
        {
          id: '5',
        },
        {
          id: '6',
        },
        {
          id: '7',
        },
        {
          id: '8',
        },
      ],
    };
  },
};
</script>

<style scoped>
.instagram__content {
  display: flex;
  justify-content: space-between;
}
.instagram__brief {
  display: flex;
  flex-direction: column;
}
.instagram__caption {
  max-width: fit-content;
  border-bottom: 3px solid #000;
  margin-bottom: 32px;
}

.instagram__desc {
  color: #666;
  max-width: 340px;
  margin: 0;
}
.instagram__grid {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  max-width: 870px;
  padding-left: 110px;
}

.instagram__grid-item {
  width: 195px;
  height: 195px;
  background-color: #ededed;
  margin: 0 30px 30px 0;
}

.instagram__grid-item:nth-of-type(4n) {
  margin-right: 0;
}

@media (max-width: 1280px) {
  .instagram__grid {
    max-width: 792px;
  }
}
</style>
