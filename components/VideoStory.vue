<template>
  <section class="video-story container ">
    <div class="video-story__content">
      <div class="video-story__text-container">
        <h2 class="video-story__caption caption caption_h2">
          Истории людей, победивших рак, но не свои привычки
        </h2>

        <p class="video-story__desc paragraph">
          Есть вещи, которые не лечатся. Вещи ставшие частью нашего «я», фобии,
          страхи. Но это точно не рак. Рак лечится. Лучшее доказательство — люди
          с их историями.
        </p>
      </div>
      <!-- Не нашел глобальных стилей подходящих для этих кнопок.
    Картинки для кнопок положил в static/img   -->

      <div class="video-story__buttons">
        <button class="video-story__button">
          <picture>
            <source srcset="/img/arrow-button-left.svg" type="image/svg+xml" />
            <img src="/img/arrow-button-left.png" alt="показать предыдущее" />
          </picture>
        </button>
        <button class="video-story__button">
          <picture>
            <source srcset="/img/arrow-button-rigth.svg" type="image/svg+xml" />
            <img src="/img/arrow-button-rigth.png" alt="показать следующее" />
          </picture>
        </button>
      </div>
    </div>
    <div class="video-story__container">
      <div class="video-story__video"></div>
      <p class="video-story__lead">
        Все видео вы можете найте на нашем
        <a href="#" class="video-story__link link"> YouTube канале.</a>
      </p>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
.video-story {
  display: flex;

  justify-content: space-between;
}
.video-story__content {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  padding: 100px 0 100px;
  margin-right: 40px;
}
.video-story__text-container {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.video-story__caption {
  margin-bottom: 32px;
}

.video-story__desc {
  max-width: 340px;
  margin: 0;
  color: #666666;
}

.video-story__buttons {
  padding-bottom: 40px;
  max-width: fit-content;
}
.video-story__button {
  width: 40px;
  height: 40px;
  background: #fbfbfb;
  border: none;
  padding: 0;
  margin-right: -5px;
  cursor: pointer;
}
.video-story__container {
  padding: 100px 0;
  display: flex;
  flex-direction: column;
}

.video-story__video {
  width: 867px;
  height: 450px;
  background: #ededed;
}
.video-story__lead {
  font-size: 12px;
  line-height: 16px;
  color: #666666;
}

.video-story__link {
  text-decoration: underline;
}

@media (max-width: 1280px) {
  .video-story__video {
    width: 773px;
    height: 400px;
    background: #ededed;
  }

  .video-story__desc {
    max-width: 305px;
  }
}
</style>
