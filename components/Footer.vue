<template>
  <container>
    <footer class="footer">
      <main-title />
    </footer>
  </container>
</template>

<script>
import MainTitle from '@/components/MainTitle';
import Container from '@/components/Container';
export default {
  'main-title': MainTitle,
  container: Container,
};
</script>

<style scoped></style>
