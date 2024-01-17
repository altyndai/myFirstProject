<template>
  <footer class="footer">
    <div class="container">
      <div class="footer-info">
        <div class="footer-services">
          <h3 class="footer__title">Услуги</h3>
          <a class="footer__subtitle" href="#">Дизайн интерьера</a>
          <a class="footer__subtitle" href="#">Ремонтные работы</a>
          <a class="footer__subtitle" href="#">Строительство коттеджей</a>
          <a class="footer__subtitle" href="#">Комплектация проектов</a>
          <a class="footer__subtitle" href="#">Натяжные потолки и остекление</a>
        </div>
        <div class="footer-Portfolio">
          <h3 class="footer__title">Портфолио</h3>
          <a class="footer__subtitle">Дизайн интерьера</a>
          <a class="footer__subtitle">Ремонтные работы</a>
          <a class="footer__subtitle">Строительство коттеджей</a>
          <a class="footer__subtitle">Видеообзоры</a>
        </div>
        <div class="footer-company">
          <h3 class="footer__title">О компании</h3>
          <p class="footer__title">Контакты</p>
          <div class="logo-icon">
            <img
              class="icon-company"
              src="../../public/img/logo-instagram.svg"
              alt=""
            />
            <img
              class="icon-company"
              src="../../public/img/logo-vk 1.svg"
              alt=""
            />
            <img
              class="icon-company"
              src="../../public/img/logo-youtube 1.svg"
              alt=""
            />
          </div>
        </div>
        <div class="footer-info__addres">
          <img
            class="footer__logo"
            src="../../public/img/logo.оригинал.в.svg"
            alt=""
          />

          <p class="information-addres">
            +7 (343) 288-58-13 <br />
            info@dom-uyta.ru
          </p>

          <p class="information-addres">
            г. Екатеринбург, Шевченко, 20 <br />
            Режим работы: 10:00-21:00
          </p>
        </div>
      </div>
      <div class="footer__title__confidentiality">
        <p class="confidentiality">
          © 2015 - 2021 Дом-Уюта <br />
          информация на сайте не является публичной офертой
        </p>
        <p class="confidentiality">Политика конфиденциальности</p>
        <p class="confidentiality">Согласие на обработку персональных данных</p>
        <p class="confidentiality"></p>
        <p class="confidentiality"></p>
      </div>
    </div>
  </footer>
</template>
<script></script>
<style setup>
.footer {
  background: var(--liner, linear-gradient(225deg, #3c3f48 0%, #15151a 100%));
}
.footer-info {
  display: flex;
  justify-content: space-between;
  padding: 52px 0px 70px 0px;
}
.footer-services {
  display: flex;
  flex-direction: column;
}
.footer__title {
  color: var(--color-styles-white, #fff);
  font-family: Gilroy;
  font-size: 22px;
  font-style: normal;
  font-weight: 400;
  line-height: 135%;
  margin-bottom: 20px;
}
.icon-company {
  padding-right: 37px;
}
.footer__subtitle {
  color: var(--color-styles-white, #fff);
  font-family: Gilroy;
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: 135%;
  margin-bottom: 20px;
}
.footer-Portfolio {
  display: flex;
  flex-direction: column;
}
.footer-company {
  display: flex;
  flex-direction: column;
}
.footer-info__addres {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
}

.footer__logo {
  width: 130.848px;
  height: 80.89px;
  margin-bottom: 30px;
}
.information-addres {
  color: var(--color-styles-white, #fff);
  font-family: Gilroy;
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: 135%;
  text-align: end;
}
.footer__title__confidentiality {
  display: flex;
  justify-content: space-between;
}
.confidentiality {
  color: var(--color-styles-white, #fff);
  font-family: Gilroy;
  font-size: 10px;
  font-style: normal;
  font-weight: 400;
  line-height: 135%;
}
</style>
