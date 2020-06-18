<template>
  <div>
    <p class="text">
      <slot></slot>
    </p>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.text {
  color: #fff;
  font-weight: normal;
  font-size: 16px;
  line-height: 28px;
}
@media screen and (max-width: 728px) {
  .text {
    font-size: 14px;
    line-height: 140%;
  }
}
</style>
