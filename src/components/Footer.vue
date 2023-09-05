<script setup>

</script>

<template>

<footer class="footer">
    <img src="/src/assets/flower-grey1.svg" alt="flower-grey1" class="flower-grey1">
    <img src="/src/assets/flower-grey2.svg" alt="flower-grey2" class="flower-grey2">
    <img src="/src/assets/photo-footer1.svg" alt="flower-grey2" class="photo-footer1">

    <div class="grey-bg"></div>
    <section class="region">
      <div class="container">
        <div class="region-inner">
          <div class="region-left">
            <h1 class="region-title">1954</h1>
            <h2 class="region-subtitle">Образование<br>Липецкой области</h2>
            <div class="region-info">
              Липецкая область была образована 6 января<br>1954 года из окраинных районов Рязанской,<br>Воронежской, Курской и Орловской областей
            </div>
          </div>
          <div class="region-right"></div>
        </div>
      </div>
    </section>

    <section class="facts">
      <div class="fact" id="first-fact">
        <div class="fact-left fact-img">
          <img src="/src/assets/fact1.svg" alt="">
        </div>
        <div class="fact-right fact-info">
          <h2 class="fact-title">Послевоенные годы</h2>
          <span class="fact-text">
            Интенсивное восстановление<br>промышленности и сельского хозяйства
          </span>
        </div>
      </div>
      <div class="fact" id="second-fact">
        <div class="fact-left fact-info">
          <span class="fact-text">
          Постройка новолипецкого металлургического<br>комбината, в которой участвовала вся страна.<br>Для возведения цехов и производств создана<br>мощная строительная база, развивалась<br>транспортная инфраструктура.
          </span>
        </div>
        <div class="fact-right fact-img">
          <img src="/src/assets/fact2.svg" alt="">
        </div>
      </div>
      <div class="fact" id="third-fact">
        <div class="fact-left fact-img">
          <img src="src/assets/fact3.svg" alt="">
        </div>
        <div class="fact-right fact-info">
          <h2 class="fact-title">
            Создан мощный<br>производственно-<br>технический потенциал.
          </h2>
          <span class="fact-text">
            4 июля 1967 г. Липецкая область была<br> награждена Орденом Ленина
          </span>
        </div>
      </div>
      <div class="fact" id="fourth-fact">
        <div class="fact-left fact-info">
          <h2 class="fact-title">
            Липецк — становится<br>полумиллионным<br>современным городом<br>с развитой<br>инфраструктурой
          </h2>
        </div>
        <div class="fact-right fact-info">
          <span class="fact-text">
            В 2006 Липецк насчитывает 2 тыс строительных<br>организаций. Введено в эксплуатацию 620,4 тыс. кв.<br>м. жилья, более половины из них - по областным<br>жилищным программам. Строительные работы<br>велись на 86 объектах социальной сферы.
          </span>
        </div>
      </div>
    </section>

  </footer>

</template>

<style scoped>

.footer {
  position: relative;
  z-index: 1
}

.grey-bg {
  background-image: url(./src/assets/bg-grey.svg);
  background-repeat: no-repeat;
  background-size: cover;
  height: 370px;
  max-height: 100vh;
  margin-top: -340px;
}

.region-inner {
  min-height: 75vh;
}

.region-left {
  width: 50%;
  display: flex;
  flex-direction: column;
  align-items: flex-end;
}

.region-right {
  width: 50%;
}

.region-title {
  color: #000;
  text-align: right;
  font-family: Unbounded;
  font-size: 180px;
  font-style: normal;
  font-weight: 400;
  line-height: 110%;
  letter-spacing: -5.4px;
  margin-bottom: 24px;
}

.region-subtitle {
  color: #000;
  text-align: right;
  font-family: Unbounded;
  font-size: 32px;
  font-style: normal;
  font-weight: 400;
  line-height: 110%; 
  letter-spacing: -0.96px;
  margin-bottom: 24px;

}

.region-info {
  color: #000;
  text-align: right;
  font-family: Onest;
  font-size: 24px;
  font-style: normal;
  font-weight: 400;
  line-height: 110%;
  letter-spacing: -0.72px;
}

/* REGION - DECOR */

.flower-grey1 {
  position: absolute;
  left: 0;
  top: 400px;
}

.flower-grey2 {
  position: absolute;
  right: 0;
  top: 50px;
}

.photo-footer1 {
  position: absolute;
  right:0;
  top: 235px;
}

/* ----- REGION - FACTS ----- */


.fact {
  height: 450px;
  display: flex;
  margin-bottom: 10px;
}

.fact-left {
  width: 50%;
  height: 100%;
}

.fact-left img {
  width: 95%;
  height: 95%;
}

.fact-right {
  width: 50%;
  height: 100%;
}

.fact-right img {
  width: 95%;
  height: 95%;
}

.fact-img {
  display: flex;
  justify-content: center;
  align-items: center;
}

.fact-info {
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.fact-title {
  color: #000;
  font-family: "Unbounded";
  font-size: 32px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
  margin-bottom: 20px;
}

.fact-text {
  color: #000;
  font-family: "Onest";
  font-size: 24px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}

#second-fact .fact-info {
  display: flex;
  align-items: center;
}

#fourth-fact .fact-info:first-child{
  display: flex;
  align-items: center;
}


</style>