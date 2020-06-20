<template>
  <container>
    <footer class="footer">
      <main-title>Свяжитесь со мной</main-title>
      <div class="footer__content">
        <div class="footer__form">
          <h3 class="footer__form-subtitle">
            Можете просто оставить заявку, я позвоню вам сегодня
          </h3>
          <input
            type="text"
            name="user-name"
            class="footer__input footer__input-nameIcon"
            placeholder="Ваше имя"
          />
          <input
            type="value"
            name="user-phone"
            class="footer__input footer__input-namePhone"
            placeholder="Ваш телефон"
          />
          <main-button class="button__big">Бесплатная консультация</main-button>
        </div>

        <div class="footer__text">
          <div class="footer__contacts">
            <div class="footer__contact">
              <h2 class="footer__subtitle">Телефон</h2>
              <p class="footer__cnt">+7 999 123 45 67</p>
            </div>
            <div class="footer__contact">
              <h2 class="footer__subtitle">Почта</h2>
              <a href="#" class="footer__cnt">ivanov@mail.ru</a>
            </div>
          </div>
          <div class="footer__social">
            <h2 class="footer__subtitle">Соцсети</h2>
            <a href="#" class="footer__social-links">t.me/ivanov</a>
            <a href="#" class="footer__social-links">vk.me/ivanov</a>
            <a href="#" class="footer__social-links">fb.me/ivanov</a>
          </div>

          <social-links />
        </div>
      </div>
    </footer>
  </container>
</template>

<script>
import MainTitle from '@/components/MainTitle';
import Container from '@/components/Container';
import SocialLinks from '@/components/SocialLinks';
import MainButton from '@/components/MainButton';
export default {
  components: {
    'main-title': MainTitle,
    container: Container,
    'social-links': SocialLinks,
    'main-button': MainButton,
  },
};
</script>

<style scoped>
.footer {
  margin-bottom: 50px;
}
/*==============================   footer__content  ================================*/
.footer__content {
  display: flex;
  flex-flow: row nowrap;
  justify-content: space-between;
}
/*==============================   footer__text  ================================*/
.footer__text {
  width: 45%;
  color: #fff;
}
.footer__contacts {
  display: flex;
  justify-content: space-between;
  padding-bottom: 40px;
}
.footer__social {
  padding-bottom: 40px;
}
.footer__subtitle {
  padding-bottom: 18px;
}
.footer__social-links {
  padding-right: 55px;
}
.footer__social-links:last-child {
  padding-right: 0;
}

.footer__social-links,
.footer__cnt {
  color: #fff;
  text-decoration: none;
}
.footer__social-links:hover,
.footer__cnt:hover {
  text-decoration: underline blue;
}
/*==============================   footer__form   ================================*/
.footer__form {
  width: 50%;
  background-color: #fff;
  text-align: center;
  justify-content: center;
  align-items: center;
  display: flex;
  flex-flow: column nowrap;
  box-shadow: -5px 5px 0 1px #e7a61a;
  border-radius: 5px;
  padding: 56px 0 47px;
}
.footer__form-subtitle {
  margin-bottom: 30px;
  width: 430px;
}
.footer__input {
  width: 380px;
  height: 70px;
  margin-bottom: 25px;
  padding-left: 40px;

  background: #f8f8f8;
  box-shadow: inset 0px 3px 10px rgba(199, 199, 199, 0.25);
  border: none;
  border-radius: 5px;
}
.footer__input-nameIcon {
  background-image: url(/user-icon.png);
  background-position: 3% 50%;
  background-repeat: no-repeat;
}
.footer__input-namePhone {
  background-image: url(/phone-icon.png);
  background-position: 3% 50%;
  background-repeat: no-repeat;
}

.footer__input:hover {
  border: blue 2px solid;
}

.button__big {
  padding: 0 55px;
}
.button__link:hover {
  text-decoration: underline blue;
}
</style>
