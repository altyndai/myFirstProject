<template>
  <!-- =================================header============================ -->
  <header class="header">
    <div class="container">
      <Navbar></Navbar>
      <swiper
        :navigation="true"
        :loop="true"
        :modules="modules"
        class="mySwiper"
      >
        <swiper-slide>
          <div class="slide">
            <h3 class="slide__title">
              Авторский дизайн интерьера и ремонт «под ключ»
            </h3>
            <p class="slide__subtitle">
              Мы - команда полного цикла. Проектируем и реализуем уникальные
              дизайнерские решения в Екатеринбурге.
            </p>
            <img
              class="slider__video"
              src="../../public/img/bunner.png"
              alt=""
            />
            <button class="slide__button">связаться</button>
          </div></swiper-slide
        ><swiper-slide>
          <div class="slide">
            <h3 class="slide__title">
              Авторский дизайн интерьера и ремонт «под ключ»
            </h3>
            <p class="slide__subtitle">
              Мы - команда полного цикла. Проектируем и реализуем уникальные
              дизайнерские решения в Екатеринбурге.
            </p>
            <img
              class="slider__video"
              src="../../public/img/bunner.png"
              alt=""
            />
            <button class="slide__button">связаться</button>
          </div></swiper-slide
        ><swiper-slide>
          <div class="slide">
            <h3 class="slide__title">
              Авторский дизайн интерьера и ремонт «под ключ»
            </h3>
            <p class="slide__subtitle">
              Мы - команда полного цикла. Проектируем и реализуем уникальные
              дизайнерские решения в Екатеринбурге.
            </p>
            <img
              class="slider__video"
              src="../../public/img/bunner.png"
              alt=""
            />
            <button class="slide__button">связаться</button>
          </div></swiper-slide
        >
      </swiper>
      <div class="description d-flex align-items-center p-4 bg">
        <ul class="description-menu d-flex me-4 d-flex align-items-center mb-0">
          <li class="description__title mx-4"><a href="#">дизайн</a></li>
          <li class="description__title mx-4"><a href="#">ремонт</a></li>
          <li class="description__title mx-4"><a href="#">коттеджи</a></li>
          <li class="description__title mx-4"><a href="#">комплектующие</a></li>
        </ul>
      </div>
    </div>
  </header>
  <!-- =================================header============================ -->
  <!-- ===================================наши услуги======================= -->
  <section class="services">
    <div class="container">
      <h2 class="services__title">Наши услуги</h2>
      <swiper
        :pagination="true"
        :modules="modules"
        :slidesPerView="4"
        :spaceBetween="22"
        class="servicesSlide"
        :breakpoints="{
          '@0.00': {
            slidesPerView: 1,
            spaceBetween: 30,
          },
          '@0.75': {
            slidesPerView: 1,
            spaceBetween: 20,
          },
          '@1.00': {
            slidesPerView: 2,
            spaceBetween: 50,
          },
          '@1.50': {
            slidesPerView: 3,
            spaceBetween: 70,
          },
        }"
      >
        <swiper-slide v-for="item in service" :key="item.id">
          <img :src="item.img" :alt="item.title" class="services-info__img" />
          <a class="services-info__title">
            {{ item.title }}
          </a>
        </swiper-slide>
      </swiper>
    </div>
  </section>
  <!-- ==========================наши услуги======================= -->

  <!-- ==========================description======================= -->
  <section class="content">
    <div class="container">
      <div class="content-info">
        <div class="content-info__box">
          <h2 class="content-info__title">Мы слышим своих заказчиков</h2>
          <p class="content-info__subtitle">
            Для нас важно максимально понять в каком именно пространстве Вам
            будет комфортно жить, делаем акцент на стиль и вкус.
          </p>
          <img
            class="content-info__image"
            src="../../public/img/Icon-Timer.svg"
            alt=" Для нас важно максимально понять в каком именно пространстве Вам
            будет комфортно жить, делаем акцент на стиль и вкус."
          />
          <img
            class="content-info__img"
            src="../../public/img/sketching 1.svg"
            alt=" Для нас важно максимально понять в каком именно пространстве Вам
            будет комфортно жить, делаем акцент на стиль и вкус."
          />
        </div>
        <div class="content__img">
          <img class="content__image" src="../../public/img/img1.png" alt="" />
        </div>
      </div>
      <!-- ========================================== -->
      <div class="content-item">
        <div class="content-item-info">
          <div class="content-photo">
            <img
              class="content-item__image"
              src="../../public/img/i1.png"
              alt=""
            />
            <img
              class="content-item__img"
              src="../../public/img/i2.png"
              alt=""
            />
          </div>

          <div class="content-info__box margin">
            <h2 class="content-info__title">
              Комплектуем <br />
              проекты
            </h2>
            <p class="content-info__subtitle title">
              В нашем салоне, мы с Вами сможем выбрать разные отделочные
              материалы. Мы подготовим план-график поставки в соответствии с
              которым закупим и доставим вам все необходимые материалы по вашему
              проекту.
            </p>
            <img
              src="../../public/img/1p.svg"
              alt=" Для нас важно максимально понять в каком именно пространстве Вам
            будет комфортно жить, делаем акцент на стиль и вкус."
            />
            <img
              class="content-info__img"
              src="../../public/img/2p.svg"
              alt=" Для нас важно максимально понять в каком именно пространстве Вам
            будет комфортно жить, делаем акцент на стиль и вкус."
            />
          </div>
        </div>
      </div>
      <!-- ========================================== -->
    </div>
  </section>
  <section class="record">
    <div class="container">
      <div class="record-info">
        <div class="record-info__box">
          <h2 class="record-info__title">
            Посетите любой из наших объектов в живую и убедитесь в качестве
            выполняемых нами работ!
          </h2>
          <swiper class="mt-5 mb-5"></swiper>
          <p class="record-info__subtitle">
            Покажем текущие проекты на разных стадиях: от идеи на фото до
            созданий готового дизайна
          </p>
        </div>
        <div class="record-info__block">
          <h2 class="record-info__block__title">Записаться на просмотр</h2>
          <div class="d-flex flex-column">
            <input
              class="record__input"
              type="text"
              placeholder="Введите ваше имя"
            /><input
              class="record__block__input"
              type="text"
              placeholder="Введите ваш телефон"
            />
          </div>
          <div class="mb-3 mt-4 ms-3 form-check">
            <input
              type="checkbox"
              class="form-check-input"
              id="exampleCheck1"
            />
            <label class="form-check-label" for="exampleCheck1"
              >Я согласен на обработку персональных данных</label
            >
          </div>
          <button type="button" class="button">ЗАПИСАТЬСЯ на просмотр</button>
        </div>
      </div>
    </div>
  </section>
  <!-- ==========================description========================= -->
  <!-- ============================Our work===================== -->
  <section class="ourWork">
    <div class="container">
      <div class="ourWork__txt">
        <h2 class="ourWork__title">Наши работы</h2>
        <ul class="ourWork__menu">
          <li><a class="ourWork__menu__a" href="#">Все</a></li>
          <li><a class="ourWork__menu__a" href="#">Дизайн</a></li>
          <li><a class="ourWork__menu__a" href="#">Ремонт</a></li>
          <li><a class="ourWork__menu__a" href="#">Коттеджи</a></li>
        </ul>
      </div>
    </div>

    <swiper
      :effect="'coverflow'"
      :grabCursor="true"
      :centeredSlides="true"
      :slidesPerView="3"
      :coverflowEffect="{
        rotate: 50,
        stretch: 0,
        depth: 100,
        modifier: 1,
      }"
      :scrollbar="{
        dragSize: 50,
        snapOnRelease: true,
      }"
      :pagination="true"
      :modules="modules"
      class="mySwiper"
      :breakpoints="{
        '@0.00': {
          slidesPerView: 1,
          spaceBetween: 30,
        },
        '@0.75': {
          slidesPerView: 1,
          spaceBetween: 20,
        },
        '@1.00': {
          slidesPerView: 2,
          spaceBetween: 50,
        },
        '@1.50': {
          slidesPerView: 3,
          spaceBetween: 70,
        },
      }"
    >
      <swiper-slide v-for="element in work" :key="element.id"
        ><img
          :src="element.img"
          :alt="element.title"
          class="ourWork-slider__img"
          :class="``"
        />
        <a class="ourWork-slider__title">
          {{ element.title }}
        </a>
      </swiper-slide>
    </swiper>
    <a class="ourWork__a" href="#">больше работ</a>
  </section>
  <!-- ============================Our work===================== -->
  <!-- =============================video======================= -->
  <section class="ourStudio">
    <div class="container">
      <div class="ourStudio-info">
        <div class="ourStudio__txt">
          <h2 class="ourStudio__title">Видеообзоры реализованных проектов</h2>
          <p class="ourStudio__subtitle">
            Наша студия реализовала более <span>500</span> проектов в
            Екатеринбурге
          </p>
        </div>
        <div class="ourStudio__video__box">
          <div
            v-for="part in video"
            :key="part.id"
            class="ourStudio__video__col"
          >
            <div class="ourStudio__video__block">
              <video class="video" width="305" height="309" controls>
                <source
                  src="../assets/видео/COSTA RICA IN 4K 60fps HDR (ULTRA HD).mp4"
                />
              </video>
              <div class="ourStudio__video__title">
                <div class="video__title">{{ part.title }}</div>
                <div class="video__subtitle">{{ part.subtitle }}</div>
              </div>
            </div>
          </div>
          <div></div>
        </div>
      </div>
    </div>
    <div class="ourStudio__video__box-slider">
      <swiper
        :pagination="true"
        :modules="modules"
        :slidesPerView="1"
        :spaceBetween="22"
        class="mySwiper"
      >
        <swiper-slide v-for="part in video" :key="part.id" class="pb-5">
          <div>
            <video controls style="width: 100%">
              <source
                src="../assets/видео/COSTA RICA IN 4K 60fps HDR (ULTRA HD).mp4"
              />
            </video>
          </div>
        </swiper-slide>
      </swiper>
    </div>
  </section>

  <!-- =============================video======================= -->
  <!-- =============================reviews===================== -->
  <section class="reviews">
    <div class="container">
      <div class="reviews__box">
        <div class="reviews__title">Отзывы</div>
        <div class="reviews__box-subtitle">
          <div class="reviews__subtitle">читать на flamp</div>
          <img src="../../public/img/Flamp.svg" alt="" />
        </div>
      </div>

      <swiper
        :cssMode="true"
        :navigation="true"
        :pagination="true"
        :mousewheel="true"
        :keyboard="true"
        :modules="modules"
        class="mySwiper"
      >
        <swiper-slide v-for="index in rewiev" :key="index.id">
          <div class="review__slide">
            <img
              class="review__slide__vector mb-5"
              src="../../public/img/Vector.svg"
              alt=""
            />
            <p class="review__slide__title">
              {{ index.title }}
            </p>

            <img
              class="rewiev__slide__vector"
              src="../../public/img/Vector2.svg"
              alt=""
            />
            <p class="rewiev__slide__subtitle">
              {{ index.subtitle }}
            </p>
          </div></swiper-slide
        >
      </swiper>
    </div>
  </section>
  <!-- =============================reviews===================== -->
  <!-- ===========================questions===================== -->
  <section class="questions">
    <div class="container">
      <div class="questions-info">
        <div class="questions-img">
          <img src="../../public/img/lamp.png" alt="" />
        </div>
        <div class="questions__txt">
          <h2 class="questions__txt__title">Вопрос-ответ</h2>
          <div
            v-for="item in accordions"
            :key="item.id"
            class="accordion accordion-flush"
            :id="item.idParent"
          >
            <div class="accordion-item">
              <h2 class="accordion-header">
                <button
                  class="accordion-button collapsed"
                  type="button"
                  data-bs-toggle="collapse"
                  :data-bs-target="`#${item.idAccordion}`"
                  aria-expanded="false"
                  :aria-controls="item.idAccordion"
                >
                  {{ item.title }}
                </button>
              </h2>
              <div
                :id="item.idAccordion"
                class="accordion-collapse collapse"
                data-bs-parent="#accordionFlushExample"
              >
                <div class="accordion-body">
                  {{ item.subtitle }}
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- ===========================questions===================== -->
  <!-- ===========================consultation================== -->
  <section class="consultation">
    <div class="container">
      <div class="consultation-info">
        <div class="consultation-info__box">
          <h2 class="consultation-info__title">
            Остались вопросы? Спросите специалиста
          </h2>
          <swiper class="mt-5"></swiper>
          <p class="consultation-info__subtitle">
            Закажите бесплатную консультацию, и через 5 минут с вами свяжется
            специалист
          </p>
        </div>
        <div class="consultation-info__block">
          <h2 class="consultation-info__block__title">
            Бесплатная консультация
          </h2>
          <div class="d-flex flex-column">
            <input
              class="consultation__input"
              type="text"
              placeholder="Введите ваше имя"
            /><input
              class="consultation__block__input"
              type="text"
              placeholder="Введите ваш телефон"
            />
          </div>
          <div class="mb-3 mt-4 ms-3 form-check">
            <input
              type="checkbox"
              class="form-check-input"
              id="exampleCheck1"
            />
            <label class="form-check-label" for="exampleCheck1"
              >Я согласен на обработку
              <a class="form-check-label" href="#"
                >персональных данных</a
              ></label
            >
          </div>
          <button type="button" class="consultation__button">
            ЗАПИСАТЬСЯ на просмотр
          </button>
        </div>
      </div>
    </div>
  </section>
  <!-- ===========================consultation================== -->
  <!-- ===========================contact================== -->
  <section class="contact">
    <div class="container">
      <div class="contact__block">
        <div class="contact-info">
          <h1 class="contact-info__title">Контакты</h1>
          <div class="contact-info__connection">
            Свяжитесь с нами
            <p class="number-email">
              +7 (343) 288-58-13 <br />
              info@dom-uyta.ru
            </p>
          </div>
          <div class="address">
            Наш адрес
            <p class="address-description">
              г. Екатеринбург, Шевченко, 20 <br />
              Режим работы: 10:00-21:00
            </p>
          </div>
        </div>
        <div class="contact__network">
          <div class="logo-icon">
            <img src="../../public/img/logo-instagram.svg" alt="" />
            <img src="../../public/img/logo-vk 1.svg" alt="" />
            <img src="../../public/img/logo-youtube 1.svg" alt="" />
          </div>
          <div class="instagram">
            <p class="instagram__title">нажми</p>
            <img class="arrow" src="../../public/img/strelka.svg" alt="" />
            <img src="../../public/img/dom_uyta2.svg" alt="" />
          </div>
        </div>
        <div class="contact__map">
          <iframe
            class="map"
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2300421.7626201552!2d71.0852738873337!3d39.98560333131973!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x38bc35b99dc9f579%3A0x4590139fc0c83acb!2z0J3QvtC-0LrQsNGC!5e0!3m2!1sru!2skg!4v1683379402356!5m2!1sru!2skg"
            style="border: 0"
            loading="lazy"
            referrerpolicy="no-referrer-when-downgrade"
          ></iframe>
        </div>
      </div>
    </div>
  </section>
  <FooterApp></FooterApp>
  <!-- ===========================contact================== -->
</template>
<script lang="ts" setup>
import Navbar from "../components/navbar.vue";
import { Swiper, SwiperSlide } from "swiper/vue";
import { Navigation, EffectCoverflow, Scrollbar } from "swiper";

// Import Swiper styles
import "swiper/css";
import "swiper/css/navigation";
import "swiper/css/effect-coverflow";
import "swiper/css/pagination";
import "swiper/css/scrollbar";
const modules = [Scrollbar, EffectCoverflow, Navigation];
const service: any[] = [
  {
    id: 1,
    img: "../public/img/1.png",
    title: "Дизайн интерьера",
  },
  {
    id: 2,
    img: "../public/img/2.png",
    title: "Ремонт квартир и домов",
  },
  {
    id: 3,
    img: "../public/img/3.png",
    title: "Строительство коттеджей",
  },
  {
    id: 4,
    img: "../public/img/4.png",
    title: "Комплектация проектов",
  },
  {
    id: 5,
    img: "../public/img/4.png",
    title: "Комплектация проектов",
  },
  {
    id: 6,
    img: "../public/img/4.png",
    title: "Комплектация проектов",
  },
];
const work: any[] = [
  {
    id: 1,
    img: "../public/img/24.png",
    title: "Дизайн интерьера в 3-к квартире",
  },
  {
    id: 2,
    img: "../public/img/14.png",
    title: "Дизайн интерьера в 3-к квартире",
  },
  {
    id: 3,
    img: "../public/img/39.png",
    title: "Дизайн интерьера в 3-к квартире",
  },
  {
    id: 4,
    img: "../public/img/24.png",
    title: "Дизайн интерьера в 3-к квартире",
  },
  {
    id: 5,
    img: "../public/img/24.png",
    title: "Дизайн интерьера в 3-к квартире",
  },
];
const video: any[] = [
  {
    id: 1,
    video: "../assets/видео/COSTA RICA IN 4K 60fps HDR (ULTRA HD).mp4",
    title: "Ремонт в ЖК Бриз",
    subtitle: "3:52",
  },
  {
    id: 2,
    video: "../assets/видео/COSTA RICA IN 4K 60fps HDR (ULTRA HD).mp4",
    title: "Ремонт по дизайн-проекту",
    subtitle: "1:44",
  },
  {
    id: 3,
    video: "../assets/видео/COSTA RICA IN 4K 60fps HDR (ULTRA HD).mp4",
    title: "Ремонт 2-к квартиры",
    subtitle: "2:35",
  },
  {
    id: 4,
    video: "../assets/видео/COSTA RICA IN 4K 60fps HDR (ULTRA HD).mp4",
    title: "Ремонт в коттедже",
    subtitle: "1:03",
  },
];
const rewiev: any[] = [
  {
    id: 1,
    title:
      "Дом уюта сделали мне шикарный ремонт в двух комнатах. Аккуратно, оперативно, никаких проблем с заполнением документов не возникло. Спасибо больше, рекомендую!",
    subtitle: "Егор Семёнов / 30.03.21",
  },
  {
    id: 2,
    title:
      "Дом уюта сделали мне шикарный ремонт в двух комнатах. Аккуратно, оперативно, никаких проблем с заполнением документов не возникло. Спасибо больше, рекомендую!",
    subtitle: "Егор Семёнов / 30.03.21",
  },
  {
    id: 3,
    title:
      "Дом уюта сделали мне шикарный ремонт в двух комнатах. Аккуратно, оперативно, никаких проблем с заполнением документов не возникло. Спасибо больше, рекомендую!",
    subtitle: "Егор Семёнов / 30.03.21",
  },
  {
    id: 4,
    title:
      "Дом уюта сделали мне шикарный ремонт в двух комнатах. Аккуратно, оперативно, никаких проблем с заполнением документов не возникло. Спасибо больше, рекомендую!",
    subtitle: "Егор Семёнов / 30.03.21",
  },
];
const accordions: any[] = [
  {
    id: 1,
    title: "Когда готовы приступить к работе?",
    subtitle:
      "С момента подписания договора в течении 3-5 дней мы приступаем к работам",
    idAccordion: "accordionFlushExample1",
    idParent: "parent",
  },
  {
    id: 2,
    title: "Есть ли возможность оплаты безналом?",
    subtitle:
      "С момента подписания договора в течении 3-5 дней мы приступаем к работам",
    idAccordion: "accordionFlushExample2",
    idParent: "parent1",
  },
  {
    id: 3,
    title: "Кто у Вас работает?",
    subtitle:
      "С момента подписания договора в течении 3-5 дней мы приступаем к работам",
    idAccordion: "accordionFlushExample3",
    idParent: "parent2",
  },
  {
    id: 4,
    title: "Может ли измениться стоимость работ?",
    subtitle:
      "С момента подписания договора в течении 3-5 дней мы приступаем к работам",
    idAccordion: "accordionFlushExample4",
    idParent: "parent3",
  },
  {
    id: 5,
    title: "Помогаете ли вы с приобретением чистовых материалов?",
    subtitle:
      "С момента подписания договора в течении 3-5 дней мы приступаем к работам",
    idAccordion: "accordionFlushExample5",
    idParent: "parent4",
  },
  {
    id: 6,
    title: "Помогаете ли вы с п?",
    subtitle:
      "С момента подписания договора в течении 3-5 дней мы приступаем к работам",
    idAccordion: "accordionFlushExample6",
    idParent: "parent5",
  },
];
// footer import
import FooterApp from "../components/footer.vue";
</script>
<style>
/* ========header==================== */
.header {
  background-color: #18191e;
  height: 788px;
}
.slider__video {
  width: 958.5px;
  height: 628px;
}
.slide {
  position: relative;
}
.slide__title {
  font-family: "Playfair Display";
  font-style: normal;
  font-weight: 900;
  font-size: 47px;
  line-height: 135%;
  text-align: right;
  color: #ffffff;
  width: 55%;
  text-align: end;
  position: absolute;
  left: 44%;
  top: 15%;
}
.slide__subtitle {
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 135%;
  color: #ffffff;
  position: absolute;
  width: 25%;
  left: 76%;
  top: 44%;
}
.slide__button {
  position: absolute;
  padding: 20px 40px;
  background: #3d3e45;
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 900;
  font-size: 12px;
  line-height: 15px;
  text-align: center;
  letter-spacing: 1.5px;
  text-transform: uppercase;

  color: #ffffff;
  left: 86%;
  bottom: 4%;
}
.description {
  width: 58%;
  background-color: #282a31;
  position: absolute;
  left: 10%;
}
.description__title {
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 900;
  font-size: 12px;
  line-height: 15px;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: #ffffff;
}
.swiper-button-next {
  top: 3% !important;
  right: 3%;
}
.swiper-button-prev {
  top: 3% !important;
  right: 8% !important;
  left: auto;
}
@media screen and (max-width: 376px) {
  .slider__video {
    width: 100%;
    object-fit: cover;
    object-position: inherit;
    height: 730px;
  }
  .slide__title {
    left: 2%;
    font-size: 28px;
    width: 100%;
    text-align: start;
    top: 20%;
  }
  .slide__subtitle {
    left: 2%;
    width: 100%;
    top: 43%;
  }
  .slide__button {
    left: 2%;
    bottom: 30%;
  }
  .description {
    display: none !important;
  }
  .header .swiper-button-next {
    display: none !important;
  }
  .header .swiper-button-prev {
    display: none !important;
  }
}
/* ========header==================== */
/* ========Наши услуги=============== */
.services {
  background-color: #34363e;
  padding-bottom: 166px;
}
.services__title {
  font-family: "Playfair Display";
  font-style: normal;
  font-weight: 900;
  font-size: 52px;
  line-height: 135%;
  color: #ffffff;
  padding: 52px 0px;
}
.services-info__img {
  height: 500px;
  width: 100%;
  object-fit: cover;
  object-position: center;
}
.services-info__title {
  position: absolute;
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 700;
  font-size: 24px;
  line-height: 100%;
  color: #ffffff;
  left: 5%;
  bottom: 5%;
  width: 68%;
}
@media screen and (max-width: 376px) {
  .services-info__img {
    height: 350px;
    object-fit: cover;
    object-position: center;
  }
  .services__title {
    font-size: 28px;
  }
}

/* ========Наши услуги=============== */
/*===========content=================  */
.content {
  background-color: #26272e;
  padding-bottom: 50px;
}
.content-info {
  display: flex;
  justify-content: space-between;
  padding-top: 196px;
  padding-bottom: 226px;
}
.content-info__box {
  width: 50%;
  padding-left: 30px;
}
.content-info__title {
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 600;
  font-size: 48px;
  line-height: 56px;
  color: #ffffff;
}
.content-info__subtitle {
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 135%;
  color: #ffffff;
  width: 58%;
  margin-top: 24px;
  margin-bottom: 64px;
}
.content-info__img {
  margin-left: 17%;
  padding-bottom: 30px;
}
.content-info__image {
  padding-bottom: 30px;
}
.content__image {
  width: 100%;
}
/* ============================= */
.content-photo {
  display: flex;
  width: 50%;
}
.content-item-info {
  display: flex;
  justify-content: space-between;
  padding-top: 196px;
  padding-bottom: 226px;
}
.content-item__img {
  padding-left: 20px;
  width: 50%;
  height: 90%;
  object-fit: cover;
  object-position: center;
}

.content-item__image {
  width: 35%;
  height: 50%;
  margin-top: 20%;
  object-fit: cover;
  object-position: center;
}
.title {
  width: 80%;
}
@media screen and (max-width: 376px) {
  .content-info {
    flex-direction: column;
  }
  .content-info__title {
    font-size: 28px;
  }
  .content-info__subtitle {
    font-size: 14px;
    width: 100%;
  }
  .content-info__box {
    width: 100%;
    padding-left: 0%;
  }
  .content-item-info {
    flex-direction: column;
  }
  .content-photo {
    width: 100%;
  }
  .content-item__img {
    width: 50%;
  }
  .content-item__image {
    margin-bottom: 20px;
  }
}
/* ============================= */
/*========content===============  */

/* =========record================ */
.record {
  background-color: #26272e;
  background-image: url(../../public/img/bg.png);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  height: 524.77px;
}
.record-info {
  display: flex;
  padding: 110px 0px;
}
.record-info__box {
  width: 50%;
}
.record-info__block {
  width: 50%;
}
.record-info__title {
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 600;
  font-size: 33px;
  line-height: 40px;
  color: #ffffff;
  width: 90%;
  margin-top: 28px;
}
.record-info__subtitle {
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 18px;
  color: #ffffff;
  width: 50%;
}
.record-info__block__title {
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 700;
  font-size: 24px;
  line-height: 32px;
  color: #ffffff;
}
.record__input {
  width: 68%;
  height: 50px;
  background: rgba(255, 255, 255, 0.1);
  border-radius: 4px;
  margin-bottom: 36px;
  padding-left: 20px;
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 24px;
  color: #ffffff;
}
.record__block__input {
  width: 68%;
  height: 50px;
  background: rgba(255, 255, 255, 0.1);
  border-radius: 4px;
  padding-left: 20px;
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 24px;
  color: #ffffff;
}
.form-check-label {
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 18px;
  color: #ffffff;
}
.button {
  background: #e1a600;
  width: 262px;
  height: 50px;
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 900;
  font-size: 12px;
  line-height: 15px;
  text-align: center;
  letter-spacing: 1.5px;
  text-transform: uppercase;

  color: #ffffff;
}
@media screen and (max-width: 376px) {
  .record {
    height: 800px;
  }
  .record-info {
    flex-direction: column;
  }
  .record-info__box {
    width: 100%;
  }
  .record-info__block {
    width: 100%;
  }
  .record__input {
    width: 100%;
  }
  .record__block__input {
    width: 100%;
  }
  .button {
    width: 200px;
    font-size: 10px;
  }
  .record-info__title {
    font-size: 28px;
    width: 100%;
    line-height: 37px;
  }
  .record-info__subtitle {
    width: 100%;
    margin-bottom: 50px;
  }
  .record-info__block__title {
    width: 100%;
    font-size: 20px;
  }
}
/* =========record================ */
/* =========Our work============== */
.ourWork {
  background-color: #26272e;
}
.ourWork__txt {
  padding-top: 250px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 116px;
}
.ourWork__title {
  font-family: "Playfair Display";
  font-style: normal;
  font-weight: 900;
  font-size: 52px;
  line-height: 135%;
  color: #ffffff;
}
.ourWork__menu {
  display: flex;
}
.ourWork__menu__a {
  margin-left: 64px;
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 900;
  font-size: 14px;
  line-height: 18px;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: #ffffff;
  opacity: 0.5;
}
.ourWork__menu__a:hover {
  opacity: inherit;
}
.ourWork-slider__img {
  position: relative;
  width: 100%;
}
.ourWork-slider__title {
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 600;
  font-size: 38px;
  line-height: 43px;
  color: #ffffff;
  position: absolute;
  z-index: 5;
  top: 50%;
  left: 20%;
  opacity: 0;
}

.ourWork__a {
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 900;
  font-size: 12px;
  line-height: 15px;
  display: flex;
  align-items: center;
  justify-content: center;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: #e1a600;
  padding-top: 50px;
}
.swiper-slide-active .ourWork-slider__title {
  transition: 0.8s;
  opacity: 1;
}
.swiper-scrollbar {
  width: 90% !important;
  margin-left: 40px !important;
  height: 2px !important ;
}
.swiper-scrollbar-horizontal {
  background-color: white;
}
@media screen and (max-width: 376px) {
  .ourWork__menu {
    display: none;
  }
  .ourWork-slider__title {
    font-size: 30px;
  }
  .ourWork__title {
    font-size: 45px;
  }
}

/* =========Our work============== */
/* ===========video=============== */
.ourStudio {
  background-color: #26272e;
  padding-top: 147px;
}
.ourStudio-info {
  display: flex;
  justify-content: space-between;
}
.ourStudio__txt {
  width: 50%;
}
.ourStudio__title {
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 600;
  font-size: 48px;
  line-height: 56px;
  color: #ffffff;
  margin-top: 148px;
  width: 50%;
  margin-bottom: 95px;
}
.ourStudio__subtitle {
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 400;
  font-size: 22px;
  line-height: 135%;
  color: #ffffff;
  width: 54%;
}
.ourStudio__video__box {
  width: 50%;
  display: flex;
  margin-left: -5px;
  flex-wrap: wrap;
}
.ourStudio__video__col {
  width: 50%;
  padding-left: 5px;
  margin-bottom: 5px;
}
.video {
  position: relative;
  background-color: #18191e5a;
  object-fit: cover;
  object-position: center;
}
.ourStudio__video__title {
  display: flex;
  justify-content: space-between;
  position: absolute;
}
.video__title {
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 700;
  font-size: 14px;
  line-height: 17px;
  color: #ffffff;
}
.video__subtitle {
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 400;
  font-size: 12px;
  line-height: 14px;
  letter-spacing: 0.6px;

  color: #ffffff;

  opacity: 0.5;
}
.ourStudio__video__box-slider {
  display: none;
}
@media screen and (max-width: 376px) {
  .ourStudio__video__box {
    display: none;
  }
  .ourStudio__txt {
    width: 100%;
  }
  .ourStudio__title {
    font-size: 35px;
  }
  .ourStudio__subtitle {
    font-size: 15px;
    width: 250px;
  }
  span {
    font-size: 25px;
    font-family: "Playfair Display";
  }
  .ourStudio__video__box-slider {
    display: flex;
  }
}

/* ===========video=============== */
/* =============reviews=========== */
.reviews {
  background-color: #26272e;
  padding-top: 130px;
  padding-bottom: 100px;
}
.reviews .swiper-button-next {
  top: 37% !important;
  right: 10% !important;
  color: white;
}
.reviews .swiper-button-prev {
  top: 40% !important;
  right: 85% !important;
  color: white;
}
.reviews__box {
  display: flex;
  justify-content: space-between;
  padding-bottom: 130px;
}
.reviews__title {
  font-family: Playfair Display;
  font-size: 47px;
  color: white;
  line-height: 63px;
  font-weight: 900;
}
.reviews__box-subtitle {
  display: flex;
  align-items: center;
}
.reviews__subtitle {
  font-family: Gilroy;
  font-size: 12px;
  font-weight: 800;
  line-height: 15px;
  letter-spacing: 1.5px;
  text-align: left;
  color: white;
  opacity: 0.6;
  margin-right: 10px;
}
.review__slide__title {
  font-family: Gilroy;
  font-size: 22px;
  font-weight: 400;
  line-height: 30px;
  letter-spacing: 0px;
  text-align: center;
  color: white;
  width: 55%;
}
.review__slide__subtitle {
  font-family: Gilroy;
  font-size: 16px;
  font-weight: 400;
  line-height: 22px;
  letter-spacing: 0px;
  text-align: left;
  color: white;
  margin-top: 50px;
  opacity: 0.6;
}
.review__slide {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.review__slide__vector {
  width: 16px;
  height: 15px;
}
@media screen and (max-width: 376px) {
  .reviews__title {
    font-size: 35px;
  }
  .reviews__subtitle {
    display: none;
  }
  .review__slide__title {
    font-size: 14px;
    width: 80%;
  }
  .reviews {
    padding-bottom: 0%;
    padding-top: 10%;
  }
  .reviews__box {
    padding-bottom: 30%;
  }
  .reviews .swiper-button-next {
    right: 1% !important;
  }
  .reviews .swiper-button-prev {
    right: 92% !important;
  }
}

/* =============reviews=========== */
/* =============questions========= */
.questions {
  background-color: #26272e;
  padding-top: 100px;
}
.questions-info {
  display: flex;
  justify-content: space-between;
}
.questions-img {
  width: 50%;
}
.questions__txt {
  width: 50%;
}
.questions__txt__title {
  font-family: "Playfair Display";
  font-size: 52px;
  font-weight: 900;
  line-height: 70px;
  letter-spacing: 0px;
  text-align: left;
  color: white;
  padding-bottom: 60px;
}
.accordion-button {
  font-family: "Gilroy";
  font-size: 24px;
  font-weight: 700;
  line-height: 32px;
  letter-spacing: 0px;
  text-align: left;
  background-color: #18191e !important;
  color: white;
  outline: none;
}
.accordion-body {
  font-family: "Gilroy";
  font-size: 22px;
  font-weight: 400;
  line-height: 30px;
  letter-spacing: 0px;
  text-align: left;
  background-color: #18191e;
  color: white !important;
  border-bottom: 2px solid white;
}

@media screen and (max-width: 376px) {
  .questions-img {
    display: none;
  }
  .questions__txt {
    width: 100%;
  }
  .questions__txt__title {
    font-size: 28px;
  }
  .accordion-button {
    font-size: 18px;
  }
  .accordion-body {
    font-size: 14px;
  }
}
.accordion-button:not(.collapsed) {
  color: white;
}
/* =============questions========= */
/* ==============consultation===== */
.consultation {
  background-image: url(../../public/img/line_background.png);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  height: 508px;
  background-color: #26272e;
}
.consultation-info {
  display: flex;
  padding: 110px 0px;
}
.consultation-info__box {
  width: 50%;
}
.consultation-info__block {
  width: 50%;
}
.consultation-info__title {
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 600;
  font-size: 33px;
  line-height: 40px;
  color: #ffffff;
  width: 70%;
  margin-top: 28px;
}
.consultation-info__subtitle {
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 18px;
  color: #ffffff;
  width: 44%;
}
.consultation-info__block__title {
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 700;
  font-size: 24px;
  line-height: 32px;
  color: #ffffff;
}
.consultation__input {
  width: 68%;
  height: 50px;
  background: rgba(255, 255, 255, 0.1);
  border-radius: 4px;
  margin-bottom: 36px;
  padding-left: 20px;
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 24px;
  color: #ffffff;
}
.consultation__block__input {
  width: 68%;
  height: 50px;
  background: rgba(255, 255, 255, 0.1);
  border-radius: 4px;
  padding-left: 20px;
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 24px;
  color: #ffffff;
}
.consultation__button {
  background: #e1a600;
  width: 262px;
  height: 50px;
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 900;
  font-size: 12px;
  line-height: 15px;
  text-align: center;
  letter-spacing: 1.5px;
  text-transform: uppercase;

  color: #ffffff;
}
@media screen and (max-width: 376px) {
  .consultation {
    height: 800px;
  }
  .consultation-info {
    flex-direction: column;
  }
  .consultation-info__box {
    width: 100%;
  }
  .consultation-info__block {
    width: 100%;
  }
  .consultation__input {
    width: 100%;
  }
  .consultation__block__input {
    width: 100%;
  }
  .consultation__button {
    width: 200px;
    font-size: 10px;
  }
  .consultation-info__title {
    font-size: 28px;
    width: 100%;
    line-height: 37px;
  }
  .consultation-info__subtitle {
    width: 100%;
    margin-bottom: 50px;
  }
  .consultation-info__block__title {
    width: 100%;
    font-size: 20px;
  }
}
/* ==============consultation===== */
/* ===============contact========= */
.contact {
  background-color: #26272e;
  padding: 50px;
}
.contact__block {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.contact-info__title {
  font-family: "Playfair Display";
  font-size: 52px;
  font-weight: 900;
  line-height: 70px;
  letter-spacing: 0px;
  text-align: left;
  color: white;
  margin-bottom: 50px;
}
.contact-info__connection {
  font-family: "Gilroy";
  font-size: 12px;
  font-weight: 900;
  line-height: 15px;
  letter-spacing: 1.5px;
  text-align: left;
  color: white;
}
.number-email {
  font-family: "Gilroy";
  font-size: 22px;
  font-weight: 400;
  line-height: 30px;
  letter-spacing: 0px;
  text-align: left;
  color: white;
  margin-top: 10px;
}
.address {
  font-family: "Gilroy";
  font-size: 12px;
  font-weight: 900;
  line-height: 15px;
  letter-spacing: 1.5px;
  text-align: left;
  color: white;
  margin-top: 50px;
}
.address-description {
  font-family: "Gilroy";
  font-size: 22px;
  font-weight: 400;
  line-height: 30px;
  letter-spacing: 0px;
  text-align: left;
  color: white;
  margin-top: 10px;
}
.contact__network {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  height: 300px;
}
.logo-icon img {
  margin-left: 20px;
}
.instagram {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  position: relative;
}
.instagram__title {
  font-family: "Gilroy";
  font-size: 12px;
  font-weight: 900;
  line-height: 15px;
  letter-spacing: 1.5px;
  text-align: center;
  color: white;
}
.arrow {
  position: absolute;
  left: 96%;
  bottom: 70%;
  z-index: 1000;
}
.map {
  width: 500px;
  height: 300px;
  flex-shrink: 0;
  border-radius: 14px;
}

/* ===============contact========= */
</style>
