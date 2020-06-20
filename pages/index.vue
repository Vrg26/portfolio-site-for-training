<template>
  <div class="page">
    <header-site />
    <cover class="page__cover" />
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
<style>
.page__cover {
  margin-top: 140px;
}
@media screen and (max-width: 768px) {
  .page__cover {
    margin-top: 55px;
  }
}
</style>
