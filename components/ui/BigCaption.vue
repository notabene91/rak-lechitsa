<template>
  <section class="big-caption bg_violet">
    <slot>Some text</slot>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
.big-caption {
  padding: 20px 0;
  text-align: center;
  display: flex;
  justify-content: center;
  align-content: center;
}
</style>
