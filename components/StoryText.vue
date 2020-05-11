<template>
  <section class="story-text">
    <div class="story-text__container">
      <p class="story-text__paragraph">
        Я из военной семьи. Отец хоть и не был военным сам, но нас всех держал в
        ежовых рукавицах. Думаю, поэтому мы и выросли такими ответственными.
      </p>
      <p class="story-text__paragraph">
        У меня дома до сих пор стоят часы в каждой комнате, хотя они и не нужны
        особо — я сам чувствую, опаздываю куда-то или нет, отстаю от нужного
        графика или опережаю. Вот такие встроенные внутренние часы! Будильник
        мне тоже не нужен — я всегда встаю раньше. Одеваюсь тоже быстро, как в
        армии, за 45 секунд.
      </p>

      <p class="story-text__paragraph strong">
        «В футболе если команда опоздала на 15 минут, ей засчитывается
        поражение».
      </p>

      <p class="story-text__paragraph">
        Опаздывать я тоже не люблю, на все встречи прихожу заранее. Если знаю,
        что могу попасть по дороге в пробку, то не еду на машине. В аэропорт
        приезжаю задолго до начала регистрации. Лучше подожду и кофе попью, чем
        опоздаю!
      </p>

      <p class="story-text__paragraph">
        Когда мне было 16 лет, мне в школе геометрию нужно было пересдавать. Я
        билеты выучил, знал абсолютно все. Пришел в нужное время, а учительница
        — нет. Ну, я какое-то время подождал ее и ушел. Потом она спрашивала:
        «Почему не дождался?». Я ответил: «В футболе если команда опоздала на 15
        минут, ей засчитывается поражение». Экзамен мне все-таки поставили!
        Сейчас если кто-то из футболистов моей команды опаздывает — начинаю
        злиться, могу и прикрикнуть потом. А если кто-то опоздал на тренировку
        перед игрой — все, подготовка насмарку. Я сразу начинаю думать тогда:
        «Значит, точно проиграем». Такая болезненная пунктуальность уже не
        лечится. В отличие от рака.
      </p>
      <!-- В блоке ниже по макету fw=500. Похоже на ошибку
    Я оставил 600.-->
      <p class="story-text__paragraph strong">
        «Сейчас если кто-то из футболистов моей команды опаздывает — начинаю
        злиться, могу и прикрикнуть потом. А если кто-то опоздал на тренировку
        перед игрой — все, подготовка насмарку. Я сразу начинаю думать тогда:
        «Значит, точно проиграем». Такая болезненная пунктуальность уже не
        лечится».
      </p>
    </div>
    <button
      id="share-button"
      name="share-button"
      class="story-text__share-button share"
    >
      Поделитесь этой статьей в своих социальных сетях &#8599;
    </button>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
.story-text {
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.story-text__container {
  max-width: 780px;
  font-size: 22px;
  line-height: 30px;
  margin: 0 auto 100px;
  padding-top: 130px;
}
.story-text__paragraph {
  margin-bottom: 10px;
}
.story-text__paragraph:last-of-type {
  margin-bottom: 0;
}

.story-text__share-button {
  width: 100%;
  max-width: 780px;
  font-family: Inter;
  font-size: 18px;
  line-height: 24px;
  color: #121212;
  padding: 30px 0;
  border: none;
  border-top: 1px solid #efefef;
  border-bottom: 1px solid #efefef;
  background-color: #fff;
  margin: 0 auto;
}

@media (max-width: 1280px) {
  .story-text__container {
    max-width: 720px;
    font-size: 20px;
    line-height: 28px;
    margin: 0 auto 90px;
    padding-top: 120px;
  }

  .story-text__share-button {
    width: 100%;
    max-width: 720px;
  }
}
</style>
