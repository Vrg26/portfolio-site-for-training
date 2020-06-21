<template>
  <div class="reason">
    <div class="offer">
      <img :src="icon" alt class="reason__icon" />
      <h2 class="reason__title">{{ name }}</h2>
      <p class="reason__text">{{ text }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: ['icon', 'name', 'text'],
};
</script>

<style scoped>
.reason__icon {
  width: 52px;
  height: 51px;
  margin-bottom: 22px;
}
.reason__title {
  font-style: normal;
  font-weight: bold;
  font-size: 24px;
  line-height: 28px;
}
@media screen and (max-width: 425px) {
  .reason__title {
    padding-bottom: 10px;
    font-size: 18px;
    line-height: 28px;
  }
}
</style>
