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
            <source
              srcset="/img/arrow--horizontal-r.svg"
              type="image/svg+xml"
            />
            <img
              src="/img/arrow--horizontal-r.png"
              srcset="
                /img/arrow--horizontal-r@2x.png 2x,
                /img/arrow--horizontal-r.png    1x
              "
              alt="показать следующее"
              class="arrow arrow_rotate arrow_inactive"
            />
          </picture>
        </button>
        <button class="video-story__button">
          <picture>
            <source
              srcset="/img/arrow--horizontal-r.svg"
              type="image/svg+xml"
            />
            <img
              src="/img/arrow--horizontal-r.png"
              srcset="
                /img/arrow--horizontal-r@2x.png 2x,
                /img/arrow--horizontal-r.png    1x
              "
              alt="показать следующее"
            />
          </picture>
        </button>
      </div>
    </div>
    <div class="video-story__container">
      <div class="video-story__video"></div>
      <p class="video-story__lead">
        Все видео вы можете найте на нашем
        <a
          href="#"
          class="video-story__link link"
          target="_blank"
          rel="nofollow"
        >
          YouTube канале.</a
        >
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
  max-width: 31%;
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
  width: 69%;
  padding: 100px 0;
  display: flex;
  flex-direction: column;
}

.video-story__video {
  max-width: 867px;
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

.arrow_rotate {
  /* зеркалим изображение */
  transform: scale(-1, -1);
}

.arrow_inactive {
  /* делаем полупрозрачным */
  filter: alpha(Opacity=25);
  opacity: 0.25;
}

@media (max-width: 1280px) {
  .video-story__video {
    max-width: 773px;
    height: 400px;
    background: #ededed;
  }

  .video-story__desc {
    max-width: 305px;
  }
}
</style>
