<template>
  <div class="container">
    <header-site />
    <cover class="container__cover" />
  </div>
</template>

<script>
import Header from '@/components/Header';
import Cover from '@/components/Cover';
export default {
  components: {
    'header-site': Header,
    cover: Cover,
  },
};
</script>

<style>
.container {
  width: 100%;
  max-width: 900px;
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
