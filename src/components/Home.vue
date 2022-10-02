<template>
  <div class="row">
    <h1>{{ msg }}</h1>
    <p>
      Softy Pinko is a professional Bootstrap 4.0 theme designed by Template Mo
      for your company at absolutely free of charge
    </p>
    <a href="#"><button class="btn">Discover more</button></a>
  </div>
  <div class="home__gallery">
    <div class="home__item">
      <div class="icon">
        <img alt="icon" src="../assets/featured-item-01.png" />
      </div>

      <div class="item__title"><h5>Modern Strategy</h5></div>
      <p>Customize anything in this template to fit your website needs</p>
    </div>
    <div class="home__item">
      <div class="icon">
        <img alt="icon" src="../assets/featured-item-01.png" />
      </div>
      <div class="item__title"><h5>Best Relationship</h5></div>
      <p>Contact us immediately if you have a question in mind</p>
    </div>
    <div class="home__item">
      <div class="icon">
        <img alt="icon" src="../assets/featured-item-01.png" />
      </div>
      <div class="item__title"><h5>Ultimate Marketing</h5></div>
      <p>You just need to tell your friends about our free templates</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "RowText",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h1,
h2,
h3,
h4,
h5,
h6 {
  margin: 40px 0 0;
  font-family: "Raleway", sans-serif;
  font-size: 36px;
  font-weight: 500;
  color: white;
}

.home__gallery {
  display: flex;
  justify-content: center;
  padding-top: 70px;
  white-space: break-spaces;
  h5 {
    font-size: 18px;
    font-weight: 500;
    font-family: "Raleway", sans-serif;
    margin: 15px 0 15px;
    color: black;
  }
  img {
    vertical-align: middle;
  }
  .home__item {
    cursor: pointer;
    display: block;
    background: rgb(255, 255, 255);
    box-shadow: rgb(0 0 0 / 10%) 0px 2px 48px 0px;
    border-radius: 20px;
    padding: 30px;
    text-align: center;
    transition: all 0.3s ease 0s;
    margin-bottom: 40px;
    margin-left: 30px;
    white-space: break-spaces;
    &:nth-child(1) {
      margin-left: 0px;
    }
    .icon {
      background: rgb(85, 96, 211);
      border-radius: 50px;
      width: 90px;
      line-height: 90px;
      margin: auto;
    }
  }
  p {
    color: rgb(75, 75, 75);
    font-size: 14px;
    font-weight: 500;
    font-family: "Raleway", sans-serif;
  }
}

.row {
  font-size: 13px;
  font-weight: 500;
  color: rgb(255, 255, 255);
  white-space: break-spaces;
  p {
    font-family: "Raleway", sans-serif;
    font-size: 15px;
    font-weight: 500;
    color: white;
    margin: 20px;
  }
  a {
    color: #c561a9;
  }
  .btn {
    cursor: pointer;
    border-radius: 20px;
    background: #c561a9;
    color: white;
    border: 0px solid;
    text-transform: uppercase;
    font-size: 13px;
    padding: 12px 20px;
  }
}
</style>
