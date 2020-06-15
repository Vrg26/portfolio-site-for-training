<template>
  <div class="page">
    <header-site />
    <cover />
    <reasons />
    <my-footer />
  </div>
</template>

<script>
import Header from '@/components/Header';
import Cover from '@/components/Cover';
import Reasons from '@/components/Reasons';
import Footer from '@/components/Footer';
export default {
  components: {
    'header-site': Header,
    cover: Cover,
    reasons: Reasons,
    'my-footer': Footer,
  },
};
</script>
<style></style>
