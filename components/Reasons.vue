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
          <li class="reasons__item" v-for="reason in reasons" :key="reason.id">
            <reason
              :icon="reason.icon"
              :name="reason.name"
              :text="reason.text"
            />
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
import Reason from '@/components/Reason';
export default {
  components: {
    'main-title': MainTitle,
    container: Container,
    'main-text': MainText,
    reason: Reason,
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
  padding-bottom: 100px;
}
.content {
  background-color: #141f35;
}

.reasons__block {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-auto-rows: minmax(auto, auto);
  grid-column-gap: 16px;
  grid-row-gap: 60px;
  padding-left: 0;
  list-style: none;
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
@media screen and (max-width: 425px) {
  .reasons {
    padding-bottom: 60px;
  }
}

@media screen and (max-width: 768px) {
  .reasons__block {
    grid-template-columns: repeat(2, 1fr);
    grid-auto-rows: minmax(auto, auto);
    grid-column-gap: 16px;
    grid-row-gap: 60px;
  }
}
@media screen and (max-width: 600px) {
  .reasons__block {
    grid-template-columns: 1fr;
    grid-auto-rows: minmax(auto, auto);
    grid-row-gap: 60px;
  }
}
</style>
