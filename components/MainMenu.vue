<template>
  <ul class="menu">
    <li class="menu__item">
      <nuxt-link exact active-class="active" to="/" class="link">
        Главная
      </nuxt-link>
    </li>
    <li class="menu__item">
      <nuxt-link active-class="active" to="/stories" class="link">
        Истории
      </nuxt-link>
    </li>
  </ul>
</template>

<script>
export default {};
</script>

<style scoped>
.menu {
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
  list-style-type: none;
  margin-block-start: 0;
  margin-block-end: 0;
  padding-inline-start: 0px;
}
.menu__item {
  margin-right: 40px;
}
.menu__item:last-of-type {
  margin-right: 0px;
}
.active,
.active:visited,
.active:hover {
  text-decoration: underline;
}
</style>
