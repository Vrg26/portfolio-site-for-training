<template>
  <section class="content">
    <container>
      <!-- Надо сделать адаптив -->
      <div class="reasons">
        <!-- Сделай этот компонент адаптивным -->
        <main-title class="main-title">Со мной удобно работать</main-title>
        <!-- Это стоит сделать списком -->
        <!-- Посмотри лекцию и почитай по v-for -->
        <ul class="reasons__block">
          <li>
            <img class="reasons__icon" :src="reasons[0].icon" alt />
          </li>
          <li>
            <h2 class="reasons__title">{{ reasons[0].name }}</h2>
          </li>
          <li>
            <main-text class="reasons__text">{{ reasons[0].text }}</main-text>
          </li>
        </ul>
      </div>
    </container>
  </section>
</template>

<script>
import MainTitle from '@/components/MainTitle';
import MainText from '@/components/MainText';
import Container from '@/components/Container';
export default {
  components: {
    'main-title': MainTitle,
    container: Container,
    'main-text': MainText,
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
  margin-top: 50px;
  color: white;
  display: flex;
  flex-flow: column nowrap;
}
.content {
  background-color: #141f35;
}

.reasons__block {
  width: 33%;
  margin-bottom: 100px;
  padding-left: 0;
  list-style: none;
}

.reasons__icon {
  width: 52px;
  height: 51px;
}
.reasons__title {
  padding-top: 22px;

  font-style: normal;
  font-weight: bold;
  font-size: 24px;
  line-height: 28px;
}
.reasons__text {
  padding-top: 35px;
}

@media screen and (max-width: 950px) {
  .reasons {
    max-width: 900px;
  }
}
@media screen and (max-width: 850px) {
  .reasons {
    margin-left: 0;
    margin-right: 20px;
  }
}
@media screen and (max-width: 675px) {
  .reasons {
    display: flex;
    flex-flow: nowrap column;
    margin-left: 0;
    margin-right: 20px;
  }
}

@media screen and (max-width: 950px) {
  .reasons__block {
    width: 33%;
  }
}
@media screen and (max-width: 850px) {
  .reasons__block {
    margin-right: 15px;
  }
}
@media screen and (max-width: 675px) {
  .reasons__block {
    margin-bottom: 50px;
  }
}

@media screen and (max-width: 425px) {
  .reasons__title {
    width: 270px;
  }
}

@media screen and (max-width: 425px) {
  .reasons__title {
    font-size: 18px;
    line-height: 28px;
  }
}
</style>
