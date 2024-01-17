<template>
  <nav class="navbar d-flex align-items-center p-4 bg-white">
    <div class="navbar__logo">
      <img src="../../public/img/logo.png" alt="" />
    </div>
    <ul class="navbar__menu d-flex align-items-center mb-0">
      <li class="mx-4"><a href="#">услуги</a></li>
      <li class="mx-4"><a href="#">портфолио </a></li>
      <li class="mx-4"><a href="#">о нас</a></li>
      <li class="mx-4"><a href="#">контакты</a></li>
    </ul>
    <img src="../../public/img/instagram.svg" alt="" />
  </nav>
</template>
<script lang="ts" setup></script>
<style>
.navbar {
  width: 75%;
}
.mx-4 a {
  font-family: "Gilroy";
  font-style: normal;
  font-weight: 900;
  font-size: 12px;
  line-height: 15px;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: #3b3b3b;
}
@media screen and (max-width: 376px) {
  .navbar__menu {
    display: none !important;
  }
  .navbar {
    width: 100%;
    padding: 8px !important;
  }
}
</style>
