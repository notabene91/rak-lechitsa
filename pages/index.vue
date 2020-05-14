<template>
  <div class="index">
    <banner />
    <div class="index__container container">
      <div class="index__item">
        <videoStory />
      </div>
      <div class="index__item">
        <bigCaption v-html="bigCaptions[0].content" />
      </div>
      <!-- временные стили до приведения всех padding в единые margin -->
      <div class="index__item" style="margin-bottom: 100px">
        <storyBlock />
      </div>
      <div class="index__item">
        <bigCaption v-html="bigCaptions[1].content" />
      </div>
      <div class="index__item">
        <instagramGrid />
      </div>
    </div>
    <div class="index__item">
      <tell />
    </div>
    <div class="index__item">
      <statistic />
    </div>
    <div class="index__item">
      <about />
    </div>
  </div>
</template>

<script>
import Banner from '@/components/Banner';
import VideoStory from '@/components/VideoStory';
import BigCaption from '@/components/ui/BigCaption';
import StoryBlock from '@/components/StoryBlock';
import InstagramGrid from '@/components/InstagramGrid';
import Tell from '@/components/Tell';
import Statistic from '@/components/Statistic';
import About from '@/components/About';

export default {
  components: {
    banner: Banner,
    videoStory: VideoStory,
    bigCaption: BigCaption,
    storyBlock: StoryBlock,
    instagramGrid: InstagramGrid,
    tell: Tell,
    statistic: Statistic,
    about: About,
  },
  data() {
    return {
      bigCaptions: [
        {
          id: 1,
          content:
            '<h2 class="caption caption_h2">И В ОТЛИЧИЕ ОТ РАКА, <span class="strong">#ЭТОНЕЛЕЧИТСЯ</span></h2>',
        },
        {
          id: 2,
          content:
            '<h2 class="caption caption_h2">РАССКАЗЫВАЙТЕ ВАШИ ИСТОРИИ В ИНСТАГРАМ<br /><span class="strong">#ЭТОНЕЛЕЧИТСЯ</span></h2>',
        },
      ],
    };
  },
};
</script>

<style>
.index__container {
  margin: 0 auto;
}
.index__item {
  /* сюда затем пренесу отступы, чтобы не использовать внутренние отступы в блоках */
  margin-bottom: 0px;
}
</style>
