<template>
  <div class="search container">
    <h1 class="search__title">Истории неизлечимых привычек</h1>
    <form class="search__form" name="search">
      <input type="text" class="search__input" />
      <button class="btn search__btn ">Поиск</button>
    </form>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.search {
  margin: 0 auto;
}
.search__title {
  max-width: 413px;
  font-weight: 600;
  font-size: 32px;
  line-height: 36px;
  padding: 100px 0 70px;
  text-align: left;
}
.search__form {
  padding-bottom: 70px;
  display: flex;
  justify-content: space-between;
}
.search__btn {
  margin-right: 0;
}
.search__input {
  border: 1px solid #e8e8e8;
  margin-right: 20px;
  width: 100%;
  min-height: 52px;
}
@media (max-width: 320px) {
}
</style>
