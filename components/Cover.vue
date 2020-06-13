<template>
  <section class="cover">
    <div class="cover__text-content">
      <p class="cover__freelancer">Фрилансер</p>
      <h1 class="cover__title">Петр Федоров</h1>
      <main-text class="cover__text"
        >разрабатываю сайты для малого и среднего бизнеса. У меня можно заказать
        дизайн и верстку небольшого сайта или интернет-магазина</main-text
      >
      <cover-button class="cover__button">Бесплатная консультация</cover-button>
    </div>
    <img class="cover__avatar" src="/avatar.png" alt="avatar" />
  </section>
</template>

<script>
import MainText from '@/components/MainText';
import MainButton from '@/components/MainButton';
export default {
  components: {
    'main-text': MainText,
    'cover-button': MainButton,
  },
};
</script>
<style scoped>
.cover {
  display: flex;
  justify-content: space-between;
}
.cover__text-content {
  max-width: 450px;
}
.cover__freelancer {
  font-size: 24px;
  line-height: 28px;
  color: #ffbb01;
}
.cover__title {
  color: #fff;
  margin-top: 20px;
  font-weight: bold;
  font-size: 50px;
  line-height: 59px;
}
.cover__text {
  margin-top: 20px;
}
.cover__button {
  margin-top: 40px;
}
.cover__avatar {
  width: 362px;
  border-radius: 50%;
  border: 11px solid #fff;
}
</style>
