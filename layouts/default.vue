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
  width: 100%;
  max-width: 1320px;
}
/* modificators */
.strong {
  font-weight: 600;
}
</style>
