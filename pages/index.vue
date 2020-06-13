<template>
  <div class="container">
    <header-site />
  </div>
</template>

<script>
import Header from '@/components/Header';
export default {
  components: {
    'header-site': Header,
  },
};
</script>

<style>
.container {
  width: 100%;
  max-width: 900px;
  margin: 0 auto;
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
