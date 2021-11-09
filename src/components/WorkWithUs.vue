<template>
  <div class="wraper text-center">
    <h1>Робота з нами</h1>
    <div class="items d-flex justify-center">
      <div class="item">
        <p>Внесення накладних з обладнанням та ліцензіями</p>
        <div class="radius_top">01</div>
      </div>
      <div class="item">
        <div class="radius_buttom">02</div>
        <p>Перегляд предметів та приміщення у якому їх встановлено</p>
      </div>
      <div class="item">
        <p>Перегляд предметів та їх власників</p>
        <div class="radius_top">03</div>
      </div>
      <div class="item">
        <div class="radius_buttom">04</div>
        <p>Перегляд обладнання з індивідуальними QR-кодами</p>
      </div>
      <div class="item">
        <p>Передача обладнання між власникам</p>
        <div class="radius_top">05</div>
      </div>
      <div class="item">
        <div class="radius_buttom">06</div>
        <p>Відправлення обладнання у ремонт</p>
      </div>
      <div class="item">
        <p>Списання обладнання</p>
        <div class="radius_top">07</div>
      </div>
      <div class="item">
        <div class="radius_buttom">08</div>
        <p>Утилізація обладнання</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "WorkWithUs",
  data: () => ({}),
};
</script>

<style scoped>
.wraper {
  font-family: "Nunito";

  background-color: rgba(67, 84, 242, 0.5);
  background: url("../assets/Vector 28.png") no-repeat center center;
  background-size: cover;
  height: 635px;

}
h1 {
  font-size: 48px;
  margin-bottom: 50px;
  margin-top: 84px;
  /* color: #00084d; */
}
.radius_buttom {


  background: #4354f2;
  border-radius: 0 0 50% 50% / 0 0 100% 100%;

  font-family: Nunito;
  font-style: normal;
  font-weight: bold;
  color: #ffffff;

  position: relative;
  top: 212px;
  font-size: 60px;
  width: 200px;
  height: 100px;
}
.radius_top {

  width: 10em;
  height: 5em;
  background: #4354f2;
  border-radius: 50% 50% 0 0 / 100% 100% 0 0; /* угол состоит из половины ширины (50% от 10em = 10em : 2 = 5em) и всей высоты (100% от 5em = 5em) */
  align-items: center;
  justify-content: center;
  font-family: Nunito;
  font-style: normal;
  font-weight: bold;
  color: #ffffff;
  font-size: 24px;
  font-size: 60px;
  position: relative;
  top: 0px;
  width: 200px;
  height: 100px;
}
p {
  width: 200px;
  height: 97px;
  text-align: center;

}
</style>
