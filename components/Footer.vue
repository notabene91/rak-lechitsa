<template>
  <footer class="footer">
    <div class="footer__container container">
      <div class="footer__line">
        <div class="footer__item">
          <p class="footer__caption caption caption_h2 strong">
            Спасибо всем, кто помог состояться этому проекту
          </p>
          <nav>
            <main-menu />
          </nav>
        </div>
      </div>
      <div class="footer__line">
        <p class="footer__copy">
          Рак Лечится 2020
        </p>
        <p class="footer__copy">
          Сделано студентами Яндекс Практикум
        </p>
      </div>
    </div>
  </footer>
</template>

<script>
import MainMenu from '@/components/MainMenu';
export default {
  components: {
    'main-menu': MainMenu,
  },
};
</script>

<style scoped>
.footer {
  padding: 60px 0;
}
.footer__container {
  margin: 0 auto;
}
.footer__line {
  display: -webkit-flex;
  display: -webkit-box;
  display: -moz-flex;
  display: -moz-box;
  display: -ms-flexbox;
  display: -ms-flex;
  display: -o-flex;
  display: flex;
  -webkit-box-pack: justify;
  -webkit-justify-content: space-between;
  -ms-flex-pack: justify;
  justify-content: space-between;
  -webkit-box-align: center;
  -webkit-align-items: center;
  -ms-flex-align: center;
  align-items: center;
  margin-bottom: 110px;
}
.footer__line:last-of-type {
  margin-bottom: 0;
}
.footer__item {
  width: 48.56%;
  display: -webkit-flex;
  display: -webkit-box;
  display: -moz-flex;
  display: -moz-box;
  display: -ms-flexbox;
  display: -ms-flex;
  display: -o-flex;
  display: flex;
  -webkit-box-pack: justify;
  -webkit-justify-content: space-between;
  -ms-flex-pack: justify;
  justify-content: space-between;
  -webkit-box-align: flex-start;
  -webkit-align-items: flex-start;
  -ms-flex-align: start;
  align-items: flex-start;
}
.footer__caption {
  display: block;
  max-width: 340px;
}
.footer__copy {
  display: block;
  font-size: 18px;
  line-height: 18px;
  color: #898989;
  margin-block-start: 0px;
  margin-block-end: 0px;
}
/* проверить почему ругается */
/deep/ .active,
/deep/ .active:visited,
/deep/ .active:hover {
  text-decoration: none;
}
</style>
