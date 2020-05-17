<template>
  <button class="big-grey-button large-btn">{{ button }}</button>
</template>

<script>
export default {
  data() {
    return {
      button: 'Больше статей',
    };
  },
};
</script>

<style scoped>
.big-grey-button {
  max-width: 100%;
  height: 82px;
  padding: 0;
  border: none;
  font-family: 'Inter', sans-serif;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 20px;
}

@media (max-width: 1280px) {
  .big-grey-button {
    height: 78px;
  }
}

@media (max-width: 1024px) {
  .big-grey-button {
    height: 50px;
    font-size: 13px;
  }
}

/* Не пойму, откуда тут mp10px. Но не просто так же? Удалять не буду :) */
@media (max-width: 320px) {
  .big-grey-button {
    margin-top: 10px;
  }
}
</style>
