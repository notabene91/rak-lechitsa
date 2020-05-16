<template>
  <section class="banner bg_violet">
    <h1 class="banner__caption caption caption_h1">
      #РАКЛЕЧИТСЯ
    </h1>
    <picture>
      <source srcset="/img/arrow--banner.svg" type="image/svg+xml" />
      <img
        src="/img/arrow--banner.png"
        alt="прокрутить вниз"
        srcset="/img/arrow--banner@2x.png 2x, /img/arrow--banner.png 1x"
      />
    </picture>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
.banner {
  /*
     тут есть подозрение, что баннер должен занимать весь экран
     height: calc(100vh - 78px);
    */
  min-height: calc(100vh - 76px);
  padding-bottom: 40px;
  /* проверить работу postcss плагина */
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  align-items: center;
}
.banner__caption {
  margin-bottom: 237px;
}
</style>
