<template>
  <section class="instagram container">
    <div class="instagram__content">
      <div class="instagram__brief">
        <h2 class="instagram__caption caption caption_h2">
          Инстаграм
        </h2>
        <p class="instagram__desc">
          Два раза в неделю мы просматриваем все посты по хештегу #этонелечится.
          Все истории, где нет нецензурных выражений и запрещенного контента
          попадают сюда. Следите за правильным написанием хештега, чтобы мы не
          пропустили вашу историю.
        </p>
      </div>
      <div class="instagram__grid">
        <!-- тут надо править под vue -->
        <div class="instagram__grid-item">
          <div class="grey-plug">Заглушка</div>
        </div>
        <div class="instagram__grid-item">
          <div class="grey-plug">Заглушка</div>
        </div>
        <div class="instagram__grid-item">
          <div class="grey-plug">Заглушка</div>
        </div>
        <div class="instagram__grid-item">
          <div class="grey-plug">Заглушка</div>
        </div>

        <div class="instagram__grid-item">
          <div class="grey-plug">Заглушка</div>
        </div>
        <div class="instagram__grid-item">
          <div class="grey-plug">Заглушка</div>
        </div>
        <div class="instagram__grid-item">
          <div class="grey-plug">Заглушка</div>
        </div>
        <div class="instagram__grid-item">
          <div class="grey-plug">Заглушка</div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  components: {},
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
  color: #666666;
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
  padding-bottom: 30px;
}

.grey-plug {
  width: 195px;
  height: 195px;
  background-color: #ededed;
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

@media (max-width: 1280px) {
  .instagram__grid {
    max-width: 792px;
  }
  .grey-plug {
    width: 171px;
    height: 171px;
  }

  .instagram__grid-item {
    padding-bottom: 27px;
  }
}
</style>
