<template>
  <section class="cover">
    <container class="cover__container">
      <div class="cover__text-content">
        <p class="cover__freelancer">Фрилансер</p>
        <h1 class="cover__title">Петр Федоров</h1>
        <main-text class="cover__text">
          разрабатываю сайты для малого и среднего бизнеса. У меня можно
          заказать дизайн и верстку небольшого сайта или интернет-магазина
        </main-text>
        <cover-button class="cover__button"
          >Бесплатная консультация</cover-button
        >
      </div>
      <div class="cover__container-avatar">
        <img class="cover__avatar" src="/avatar.png" alt="avatar" />
      </div>
    </container>
  </section>
</template>

<script>
import MainText from '@/components/MainText';
import MainButton from '@/components/MainButton';
import Container from '@/components/Container';
export default {
  components: {
    'main-text': MainText,
    'cover-button': MainButton,
    container: Container,
  },
};
</script>
<style scoped>
.cover__container {
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
.cover__container-avatar {
  max-width: 362px;
}
.cover__avatar {
  width: 100%;
  border-radius: 50%;
  border: 11px solid #fff;
}
@media screen and (max-width: 768px) {
  .cover__container {
    flex-direction: column-reverse;
    align-items: center;
    text-align: center;
  }
  .cover__title {
    font-size: 36px;
    line-height: 38px;
  }
  .cover__container-avatar {
    max-width: 262px;
  }
  .cover__avatar {
    border: 8px solid #fff;
  }
}
@media screen and (max-width: 425px) {
  .cover__title {
    font-size: 24px;
    line-height: 28px;
    margin-top: 5px;
  }
  .cover__text {
    margin-top: 15px;
  }
  .cover__avatar {
    border: 5px solid #fff;
  }
  .cover__container-avatar {
    max-width: 107px;
  }
  .cover__freelancer {
    font-size: 16px;
    line-height: 27px;
    color: #ffbb01;
    margin-top: 20px;
  }
}
</style>
