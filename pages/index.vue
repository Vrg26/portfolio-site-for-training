<template>
  <div class="page">
    <header-site />
    <cover />
    <container />
  </div>
</template>

<script>
import Header from '@/components/Header';
import Cover from '@/components/Cover';
import Container from '@/components/Container';
export default {
  components: {
    'header-site': Header,
    cover: Cover,
    container: Container,
  },
};
</script>
<style></style>
