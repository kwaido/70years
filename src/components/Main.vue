<script setup>

</script>

<template>

<div class="main">

<section class="promo">
  <img src="/src/assets/first-baloon.svg" alt="baloon" class="first-baloon">
  <img src="/src/assets/second-baloon.svg" alt="baloon" class="second-baloon">
  
  <div class="container">
    <div class="promo-inner">
      <img src="/src/assets/logo-main.svg" alt="logo">
      <img src="/src/assets/text-main.svg" alt="logo">
    </div>
  </div>
</section>

<section class="holiday">
  <img src="/src/assets/first-flower.svg" alt="flower" class="first-flower">
  <img src="/src/assets/second-flower.svg" alt="flower" class="second-flower">
  <img src="/src/assets/photo-first.svg" alt="flower" class="photo-first">

  <div class="container">
    <div class="holiday-inner">
      <div class="holiday-inner__left">
        <h1 class="holiday-title">Праздник<br>длиною<br>в 365 дней</h1>
        <h2 class="holiday-subtitle">Мотивационный текст о принятии<br>участия в праздновании юбилея</h2>
        <button class="holiday-button">подробнее</button>
      </div>
      <div class="holiday-inner__right"></div>
    </div>
  </div>
</section>

<section class="congratulations">
  <img src="/src/assets/bg-face.svg" alt="" class="bg-face">
  <img src="/src/assets/face.svg" alt="" class="face">
  <img src="/src/assets/third-flower.svg" alt="" class="third-flower">
  <img src="/src/assets/fourth-flower.svg" alt="" class="fourth-flower">
  

  <div class="green-bg"></div>          
  <div class="congrats-block">
    <div class="container">
      <div class="congrats-inner">
        <div class="congrats-inner__left"></div>
        <div class="congrats-inner__right">
          <h1 class="congrats-title">Поздравление губернатора</h1>
          <p1 class="congrats-text">
            От всей души поздравляю вас с 70-летием образования нашей<br>замечательной области! Это великолепный юбилей, который<br>отмечает не только достижения и прогресс, но и дух,<br>солидарность и сильное единство нашего края.<br><br>
            За эти семь десятилетий Липецкая область превратилась в одну<br>из самых развитых и процветающих территорий России.
          </p1>
          <div class="person">
            <img src="/src/assets/sign.svg" alt="sign" class="sign">
            <span class="name">Артамонов<br>Игорь Георгиевич</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

</div>

</template>

<style scoped>

.promo {
  background-image: linear-gradient(180deg, #67A9FF -24.07%, rgba(106, 139, 182, 0.00) 97.33%), url(./src/assets/background.png);
  background-repeat: no-repeat;
  background-size: cover;
}

.promo-inner {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  padding-bottom: 30px;
}

.promo-inner img:nth-child(1) {
  margin-right: 40px;
}

/* PROMO - DECOR */

.first-baloon {
  position: absolute;
  right: 19%;
  top: 50px;
}

.second-baloon {
  position: absolute;
  left: 10%;
  top: 530px;
  z-index: 1;
}

/* ----- HOLIDAY ----- */


.holiday {
  background-image: url(./src/assets/bg-white.svg);
  background-repeat: no-repeat;
  background-size: cover;
  min-height: 100vh;
  margin-top: -285px;
  position: relative;
}

.holiday-inner {
  padding-top: 373px;
}

.holiday-inner__left {
  width: 50%;
  display: flex;
  flex-direction: column;
  padding-right: 100px;
}

.holiday-title {
  color: #000;
  text-align: right;
  font-family: Unbounded;
  font-size: 48px;
  font-style: normal;
  font-weight: 400;
  line-height: 110%; 
  letter-spacing: -1.44px;
  margin-bottom: 40px;
}

.holiday-subtitle {
  color: #000;
  text-align: right;
  font-family: "Onest";
  font-size: 18px;
  font-style: normal;
  font-weight: 300;
  line-height: 140%; 
  letter-spacing: -0.54px;
  margin-bottom: 40px;
}

.holiday-button {
  color: #000;
  text-align: center;
  font-family: Unbounded;
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
  letter-spacing: -0.54px;

  padding: 20px 40px 23px 40px;
  border-radius: 99px;
  background: #A1E224;
  border: 0;
  align-self: flex-end;
}

/* HOLIDAY - DECOR */

.first-flower {
  position: absolute;
  right: 0;
  top: -90px;
  z-index: 1;
}
.second-flower {
  position: absolute;
  left: 0;
  top: 210px;
}

.photo-first {
  position: absolute;
  right: 0;
  top: 280px;
}


/* ----- CONGRATULATIONS ----- */


.congratulations {
  position: relative;
  z-index: 1;
}

.green-bg {
  background-image: url(./src/assets/bg-green.svg);
  background-repeat: no-repeat;
  background-size: cover;
  min-height: 100vh;
  margin-top: -120px;
  position: relative;
}

.congrats-block {
  min-height: 120vh;
  background-color: #A1E224;
  margin-top: -190px;
}

.congrats-inner {
  background-color: #fff;
  height: 570px;
  position: relative;
  z-index: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: -360px;
  border-radius: 64px;
}

.congrats-inner__left {
  width: 50%;
}

.congrats-inner__right {
  width: 50%;
  padding-left: 40px;
  
}

.congrats-title {
  color: #000;
  font-family: "Unbounded";
  font-size: 48px;
  font-style: normal;
  font-weight: 400;
  line-height: 110%; 
  letter-spacing: -1.44px;
  margin-bottom: 40px;
}

.congrats-text {
  color: #000;
  font-family: "Onest";
  font-size: 18px;
  font-style: normal;
  font-weight: 300;
  line-height: 140%;
  letter-spacing: -0.54px;
  
}

.person {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-top: 20px;
}

.sign {
  padding-left: 100px;
}

.name {
  color: #000;
  text-align: right;
  font-family: "Unbounded";
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: 130%; 
  letter-spacing: -0.54px;
  text-align: right;
  padding-right: 140px;
}

/* CONGRATS - DECOR */

.bg-face {
  position: absolute;
  top: 310px;
  left: 90px;
  z-index: 1;
}

.face {
  position: absolute;
  top: 303px;
  left: 83px;
  z-index: 2;
}

.third-flower {
  position: absolute;
  top: 225px;
  left: 0px;
  z-index: 1;
}

.fourth-flower {
  position: absolute;
  left: 600px;
  top: 745px;
  z-index: 1;
}

</style>