<template>
  <h2 class="main-title">
    <slot></slot>
  </h2>
</template>

<script>
export default {};
</script>

<style scoped>
.main-title {
  width: 700px;

  padding-top: 64px;
  padding-bottom: 80px;

  font-weight: bold;
  font-size: 36px;
  line-height: 42px;

  color: #ffffff;
}
@media screen and (max-width: 425px) {
  .main__title {
    width: 270px;
    font-size: 19px;
    line-height: 22px;
  }
}
</style>
