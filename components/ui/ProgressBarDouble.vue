<template>
  <div class="progress-bar-double">
    <div class="progress-bar-double__old">
      <div
        class="progress-bar-double__fill"
        :style="{ width: (oldBarValue / maxBarValue) * 100 + '%' }"
      ></div>
    </div>
    <div class="progress-bar-double__new">
      <div
        class="progress-bar-double__fill progress-bar-double__fill_violet"
        :style="{ width: (currentBarValue / maxBarValue) * 100 + '%' }"
      ></div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['currentBarValue', 'maxBarValue', 'oldBarValue'],
};
</script>

<style scoped>
.progress-bar-double {
  position: relative;
  width: 260px;
  height: 40px;
  margin-bottom: 20px;
}

.progress-bar-double__fill {
  height: 50%;
  position: absolute;
  display: block;
  top: 0;
  left: 0;
  background-color: #f4f4f4;
}

.progress-bar-double__fill_violet {
  top: 50%;
  left: 0;
  background-color: #613a93;
}
</style>
