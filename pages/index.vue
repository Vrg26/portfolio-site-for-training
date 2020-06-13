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
</style>
