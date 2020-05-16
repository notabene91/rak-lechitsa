<template>
  <div class="progress-bar">
    <div
      class="progress-bar__fill"
      :style="{ width: (currentBarValue / maxBarValue) * 100 + '%' }"
    ></div>
  </div>
</template>

<script>
export default {
  props: ['currentBarValue', 'maxBarValue'],
};
</script>

<style scoped>
.progress-bar {
  position: relative;
  width: 260px;
  height: 40px;
  margin-bottom: 20px;
  background-color: #f4f4f4;
}

.progress-bar__fill {
  height: 100%;
  position: absolute;
  display: block;
  top: 0;
  left: 0;
  background-color: #613a93;
}
</style>
