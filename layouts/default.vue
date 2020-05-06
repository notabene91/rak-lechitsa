<template>
  <div>
    <i-header />
    <nuxt />
  </div>
</template>

<script>
import Header from '@/components/Header';
export default {
  components: {
    'i-header': Header,
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
}
.btn:hover {
  opacity: 0.9;
}
.large-btn,
.large-btn:hover,
.large-btn:visited {
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
  font-weight: 600;
}
</style>
