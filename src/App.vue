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
.container {
  width: 100%;
  max-width: 1170px;
  margin: 0 auto;
}
.header {
  padding-top: 30px;
  nav {
    background: rgb(255, 255, 255);
    border-radius: 40px;
    padding: 25px 15px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: "Raleway", sans-serif;
    .header__nav {
      padding-left: 40px;
      &:nth-child(2) {
        padding-left: 150px;
      }
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

      &.router-link-exact-active {
        color: #c365c8;
      }
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
