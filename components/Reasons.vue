<template>
  <!-- Цвет фона должен быть другой -->
  <!-- Надо сделать адаптив -->
  <div class="reasons">
    <!-- Сделай этот компонент адаптивным -->
    <main-title class="main-title">Со мной удобно работать</main-title>
    <!-- Это стоит сделать списком -->
    <!-- Посмотри лекцию и почитай по v-for -->
    <div class="reasons__block">
      <img class="reasons__icon" :src="reasons[0].icon" alt />
      <h2 class="reasons__title">{{ reasons[0].name }}</h2>
      <!-- Я сделал компонет MainText, ты можешь его использовать тут, он по font-size адаптивный уже -->
      <p class="reasons__text">{{ reasons[0].text }}</p>
    </div>
    <div class="reasons__block">
      <img class="reasons__icon" :src="reasons[1].icon" alt />
      <h2 class="reasons__title">{{ reasons[1].name }}</h2>
      <p class="reasons__text">{{ reasons[1].text }}</p>
    </div>
    <div class="reasons__block">
      <img class="reasons__icon" :src="reasons[2].icon" alt />
      <h2 class="reasons__title">{{ reasons[2].name }}</h2>
      <p class="reasons__text">{{ reasons[2].text }}</p>
    </div>
    <div class="reasons__block">
      <img class="reasons__icon" :src="reasons[3].icon" alt />
      <h2 class="reasons__title">{{ reasons[3].name }}</h2>
      <p class="reasons__text">{{ reasons[3].text }}</p>
    </div>
    <div class="reasons__block">
      <img class="reasons__icon" :src="reasons[4].icon" alt />
      <h2 class="reasons__title">{{ reasons[4].name }}</h2>
      <p class="reasons__text">{{ reasons[4].text }}</p>
    </div>
    <div class="reasons__block">
      <img class="reasons__icon" :src="reasons[5].icon" alt />
      <h2 class="reasons__title">{{ reasons[5].name }}</h2>
      <p class="reasons__text">{{ reasons[5].text }}</p>
    </div>
  </div>
</template>

<script>
import MainTitle from '@/components/MainTitle';
// Ты не используешь этот компонент, посмотри, как я это делаю в cover
import Container from '@/components/Container';
export default {
  components: {
    'main-title': MainTitle,
    container: Container,
  },

  data() {
    return {
      reasons: [
        {
          id: '1',
          icon: 'Reason-img/offer-img.svg',
          name: 'По договору',
          text:
            ' Предоставлю все документы для бухгалтерии: договоры, счета и акты. Работаю как ИП без НДС.',
        },
        {
          id: '2',
          icon: 'Reason-img/deadline-img.svg',
          name: 'Точно в срок',
          text:
            ' В договоре прописана моя ответственность за срок проекта. Если просрочу — плачу неустойку.',
        },
        {
          id: '3',
          icon: 'Reason-img/agreement-img.svg',
          name: 'Ценник под вас',
          text:
            ' Если у вас нетиповой проект, сделаю рассчет цены за работу и объясню, как складывается цена.',
        },
        {
          id: '4',
          icon: 'Reason-img/steps-img.svg',
          name: 'Промежуточные итоги',
          text:
            ' Показываю работу поэтапно, а не в последий момент перед крайним сроком.',
        },
        {
          id: '5',
          icon: 'Reason-img/storage-img.svg',
          name: 'Хостинг и домен',
          text:
            ' Если мы договорились о цене проекта, в неё входит всё: домен и хостинг на год + SSL сертификат.',
        },
        {
          id: '6',
          icon: 'Reason-img/conversation-img.svg',
          name: 'Не брошу после сдачи',
          text:
            'Научу вас или вашего сотрудника пользоваться сайтом, запишу видео-инструкции.',
        },
      ],
    };
  },
};
</script>

<style scoped>
.reasons {
  color: white;
  display: flex;
  flex-flow: row wrap;
  width: 100%;
  /* У нас есть компонент container */
  max-width: 950px;
  margin: 0 auto;
}

.reasons__block {
  width: 300px;
  margin-bottom: 100px;
}
.reasons__icon {
  width: 52px;
  height: 51px;
}
.reasons__title {
  width: 300px;
  height: 30px;
  padding-top: 22px;

  font-style: normal;
  font-weight: bold;
  font-size: 24px;
  line-height: 28px;
}
.reasons__text {
  width: 300px;
  height: 90px;
  padding-top: 35px;
}
</style>
