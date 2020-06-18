<template>
  <div>
    <button class="button">
      <slot></slot>
    </button>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.button {
  padding: 24px 42px;
  background-color: #ffbb01;
  border: none;
  box-shadow: 0px 4px 0px #b68500;
  border-radius: 5px 5px 10px 10px;
  font-size: 12px;
  font-weight: bold;
  line-height: 14px;
  color: #1b2944;
  text-align: center;
  text-transform: uppercase;
}
@media screen and (max-width: 728px) {
  .button {
    width: 100%;
    padding: 24px 28px;
  }
}
@media screen and (max-width: 425px) {
  .button {
    font-size: 10px;
    padding: 14px 28px;
  }
}
</style>
