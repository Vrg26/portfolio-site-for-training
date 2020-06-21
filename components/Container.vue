<template>
  <div class="container">
    <slot></slot>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.container {
  width: 100%;
  max-width: 950px;
  margin: 0 auto;
}
.container__cover {
  margin-top: 140px;
}
@media screen and (max-width: 950px) {
  .container {
    padding: 0 40px 0;
  }
}
@media screen and (max-width: 425px) {
  .container {
    padding: 0 25px 0;
  }
}
</style>
