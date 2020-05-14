<template>
  <section class="story-title container">
    <div class="story-title__content">
      <div class="story-title__picture">
        <div class="grey-plug">Заглушка</div>
      </div>
      <div class="story-title__info">
        <blockquote class="story-title__quote">
          <span class="story-title__quote-accent">Александр Тарханов:</span> «Я
          не могу победить свою пунктуальность в отличии от рака»
        </blockquote>
        <div class="story-title__info-picture">
          <div class="grey-plug">Заглушка</div>
        </div>

        <div class="story-title__info-bottom">
          <a href="#" class="story-title__link link">Поделитесь ↗</a>
          <p class="story-title__date">20 апреля 2018</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
.story-title {
  margin: 0 auto;
}
.story-title__content {
  padding: 100px 0 30px;
  display: flex;
  justify-content: space-between;
}

.story-title__picture {
  margin-right: 60px;
  max-width: 580px;
  background-color: #ededed;
}

.story-title__info-picture {
  display: none;
}

.grey-plug {
  background-color: #ededed;
  width: 580px;
  height: 580px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: center;
}
.story-title__info {
  padding: 30px 0 30px;
  border-top: 1px solid #efefef;
  border-bottom: 1px solid #efefef;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.story-title__quote-accent {
  font-weight: 500;
}
.story-title__quote {
  font-size: 38px;
  line-height: 48px;
  margin: 0;
}
.story-title__info-bottom {
  display: flex;
  justify-content: space-between;
}
.story-title__link {
  font-family: Inter;
  font-size: 18px;
  line-height: 24px;
  color: #121212;
  text-decoration: none;
}

.story-title__date {
  margin: 0;
  color: #121212;
}

@media (max-width: 1280px) {
  .grey-plug {
    width: 518px;
    height: 518px;
  }

  .story-title__quote {
    font-size: 34px;
    line-height: 44px;
  }

  .story-title__info-picture {
    display: none;
  }
}

@media (max-width: 1024px) {
  .grey-plug {
    width: 407px;
    height: 407px;
  }

  .story-title__quote {
    font-size: 30px;
    line-height: 38px;
  }
  .story-title__link {
    font-size: 16px;
  }

  .story-title__date {
    font-size: 16px;
  }

  .story-title__info {
    padding: 20px 0 20px;
  }

  .story-title__picture {
    margin-right: 40px;
  }

  .story-title__info-picture {
    display: none;
  }
}

@media (max-width: 768px) {
  .grey-plug {
    width: 420px;
    height: 420px;
  }

  .story-title__quote {
    font-size: 30px;
    line-height: 38px;
    text-align: center;
  }
  .story-title__link {
    font-size: 16px;
  }

  .story-title__date {
    font-size: 16px;
  }

  .story-title__info {
    padding: 20px 0 20px;
  }

  .story-title__picture {
    margin-right: 40px;
    display: none;
  }
  .story-title__info-picture {
    display: block;
    margin: 60px auto;
  }
}

@media (max-width: 320px) {
  .grey-plug {
    width: 420px;
    height: 420px;
  }

  .story-title__quote {
    font-size: 18px;
    line-height: 21px;
    text-align: center;
  }
  .story-title__link {
    font-size: 13px;
    line-height: 16px;
  }

  .story-title__date {
    font-size: 13px;
    line-height: 16px;
  }

  .story-title__info {
    padding: 20px 0 20px;
  }

  .story-title__picture {
    margin-right: 40px;
    display: none;
  }
  .story-title__info-picture {
    display: block;
    margin: 30px auto;
  }
}
</style>
