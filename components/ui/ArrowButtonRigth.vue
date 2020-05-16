<template>
  <picture>
    <source srcset="/img/arrow--horizontal-r.svg" type="image/svg+xml" />
    <img
      src="/img/arrow--horizontal-r.png"
      srcset="
        /img/arrow--horizontal-r@2x.png 2x,
        /img/arrow--horizontal-r.png    1x
      "
      alt="показать следующее"
      class="arrow"
    />
  </picture>
</template>

<script>
export default {};
</script>

<style scoped>
.arrow_rotate {
  /* зеркалим изображение */
  transform: scale(-1, -1);
}

.arrow_inactive {
  /* делаем полупрозрачным */
  filter: alpha(Opacity=25);
  opacity: 0.25;
}
</style>
