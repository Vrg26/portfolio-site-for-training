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
</style>
