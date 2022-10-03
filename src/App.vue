<template>
  <div class="welcome">
    <div class="container">
      <div class="header">
        <nav>
          <a href="#" class="header__logo">
            <img alt="logo" src="../src/assets/logo.png" />
          </a>
          <a class="header__nav" href="">Home</a>
          <a class="header__nav" href="">About</a>
          <a class="header__nav" href="">Work Process</a>
          <a class="header__nav" href="">Testimonials</a>
          <a class="header__nav" href="">Pricing Tables</a>
          <a class="header__nav" href="">Blog Entries</a>
          <a class="header__nav" href="">Contact Us</a>
        </nav>
      </div>
      <router-view />
    </div>
  </div>
</template>

<style lang="scss">
body {
  margin: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin: 0;
}
h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: "Raleway", sans-serif;
  font-size: 14px;
  font-weight: 500;
  color: white;
}
a {
  font-size: 13px;
  font-weight: 500;
  color: black;
  text-decoration: none;
}
nav {
  background: rgb(255, 255, 255);
  border-radius: 40px;
  padding: 25px 15px;
  align-items: center;
  justify-content: center;
  font-family: "Raleway", sans-serif;
  display: flex;
}

.container {
  width: 100%;
  max-width: 1170px;
  margin: 0 auto;
}
.header {
  padding-top: 30px;
  width: 1100px;
  display: flex;
  flex-direction: column-reverse;
  align-items: flex-end;

  @media (max-width: 1150px) {
    width: 900px;
    flex-direction: column-reverse;
    align-items: flex-end;
  }
  @media (max-width: 900px) {
    width: 600px;
    /* Кнопка выпадающего списка */
    .dropbtn {
      background-color: #4caf50;
      color: white;
      padding: 16px;
      font-size: 16px;
      border: none;
    }

    /* Контейнер <div> - необходим для размещения выпадающего содержимого */
    .dropdown {
      position: relative;
      display: inline-block;
    }

    /* Выпадающее содержимое (скрыто по умолчанию) */
    .dropdown-content {
      display: none;
      position: absolute;
      background-color: #f1f1f1;
      min-width: 160px;
      box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
      z-index: 1;
    }

    /* Ссылки внутри выпадающего списка */
    .dropdown-content a {
      color: black;
      padding: 12px 16px;
      text-decoration: none;
      display: block;
    }

    /* Изменение цвета выпадающих ссылок при наведении курсора */
    .dropdown-content a:hover {
      background-color: #ddd;
    }

    /* Показать выпадающее меню при наведении курсора */
    .dropdown:hover .dropdown-content {
      display: block;
    }

    /* Изменение цвета фона кнопки раскрывающегося списка при отображении содержимого раскрывающегося списка */
    .dropdown:hover .dropbtn {
      background-color: #3e8e41;
    }
  }
  &__nav {
    padding-left: 40px;
    &:nth-child(2) {
      padding-left: 150px;
    }
  }
}
.welcome {
  background-image: url(/src/assets/banner-bg.png);
  background-repeat: no-repeat;
  background-position: center center;
  background-size: cover;
}
</style>
