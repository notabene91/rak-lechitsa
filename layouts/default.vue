<template>
  <div>
    <!--
      Нужно проверсить слушатели из Header
    <overlay />
    <popup />
    -->
    <i-header />
    <nuxt />
    <i-footer />
  </div>
</template>

<script>
import Overlay from '@/components/ui/Overlay';
import PopUp from '@/components/PopUp';
import Header from '@/components/Header';
import Footer from '@/components/Footer';
export default {
  components: {
    'i-header': Header,
    'i-footer': Footer,
    overlay: Overlay,
    popup: PopUp,
  },
};
</script>

<style>
/* blocks */
html {
  background: white;
  color: black;
  font-family: 'Inter', sans-serif;
  font-style: normal;
  font-weight: normal;
  font-size: 18px;
  line-height: 24px;
}
body {
  margin: 0;
}
.container {
  max-width: 1320px;
}

/* elements */
.caption {
  margin-block-start: 0px;
  margin-block-end: 0px;
}
.caption_h1 {
  font-weight: 800;
  font-size: 92px;
  line-height: 111px;
  text-align: center;
}
.caption_h2 {
  font-weight: 600;
  font-size: 32px;
  line-height: 36px;
}
.caption_big-caption {
  max-width: 750px;
  text-align: center;
  font-size: 30px;
  line-height: 46px;
  font-weight: normal;
}
.paragraph {
  font-size: 18px;
  line-height: 22px;
}

.btn,
.btn:visited {
  padding: 17px 44px;
  background: #613a93;
  color: white;
  cursor: pointer;
  font-weight: 500;
  font-size: 16px;
  line-height: 19px;
  text-align: center;
  text-decoration: none;
  border-style: none;
}
.btn:hover {
  opacity: 0.9;
}
.large-btn,
.large-btn:hover,
.large-btn:visited {
  width: 100%;
  display: -webkit-flex;
  display: -webkit-box;
  display: -moz-flex;
  display: -moz-box;
  display: -ms-flexbox;
  display: -ms-flex;
  display: -o-flex;
  display: flex;
  -webkit-box-pack: center;
  -webkit-justify-content: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -webkit-align-items: center;
  -ms-flex-align: center;
  align-items: center;
  cursor: pointer;
  background: #fbfbfb;
  text-decoration: none;
  padding: 31px 0;
}
.num-btn,
.num-btn:hover .num-btn:visited {
  width: 58px;
  display: -webkit-flex;
  display: -webkit-box;
  display: -moz-flex;
  display: -moz-box;
  display: -ms-flexbox;
  display: -ms-flex;
  display: -o-flex;
  display: flex;
  -webkit-box-pack: center;
  -webkit-justify-content: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -webkit-align-items: center;
  -ms-flex-align: center;
  align-items: center;
  cursor: pointer;
  background: #fbfbfb;
  text-decoration: none;
  font-weight: 500;
  font-size: 18px;
  line-height: 22px;
  padding: 20px 0;
}

.num-btn.num-btn_active {
  background: #f4f4f4;
}

.link,
.link:hover,
.link:visited {
  color: inherit;
  text-decoration: none;
}
.link:hover {
  opacity: 0.8;
}

/* modificators */
.strong {
  font-weight: 900;
}
.bg_violet {
  background: #613a93;
  color: white;
}
.share {
  cursor: pointer;
}

/* media queries  */
@media (max-width: 1280px) {
  .container {
    max-width: 1180px;
  }
  .caption_h1 {
    font-weight: 800;
    font-size: 78px;
    line-height: 94px;
  }
  .caption_h2 {
    font-weight: 600;
    font-size: 28px;
    line-height: 32px;
  }

  /* Не знаю, что это такое */
  .caption_big-caption {
    max-width: 750px;
    font-size: 30px;
    line-height: 46px;
    font-weight: normal;
  }

  /* Есть некоторые сомнениея, что стоит менять ниже шрифт. Кое-где он остался как в 1440 */
  .paragraph {
    font-size: 16px;
    line-height: 20px;
  }
}

@media (max-width: 1024px) {
  .container {
    max-width: 924px;
  }

  .caption_h2 {
    font-weight: 600;
    font-size: 24px;
    line-height: 28px;
  }

  /* Не знаю, что это такое */
  .caption_big-caption {
    max-width: 750px;
    font-size: 30px;
    line-height: 46px;
    font-weight: normal;
  }

  /* Есть некоторые сомнение, что стоит менять ниже шрифт.*/
  .paragraph {
    font-size: 13px;
    line-height: 16px;
  }
}

@media (max-width: 768px) {
  .container {
    max-width: 688px;
  }
  .caption_h1 {
    font-weight: 800;
    font-size: 64px;
    line-height: 77px;
  }
  .caption_h2 {
    font-weight: 600;
    font-size: 24px;
    line-height: 28px;
  }

  /* Синий заголовок */
  .caption_big-caption {
    max-width: 750px;
    font-size: 30px;
    line-height: 46px;
    font-weight: normal;
  }

  .strong {
    font-weight: 600;
  }
}

@media (max-width: 320px) {
  .container {
    max-width: 290px;
  }
  .caption_h1 {
    font-weight: 800;
    font-size: 36px;
    line-height: 44px;
  }
  .caption_h2 {
    font-weight: 600;
    font-size: 18px;
    line-height: 21px;
  }

  /* это синий заголовок */
  .caption_big-caption {
    max-width: 750px;
    font-size: 30px;
    line-height: 46px;
    font-weight: normal;
  }
}
</style>
