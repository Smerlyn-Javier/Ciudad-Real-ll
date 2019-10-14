<template>
  <div class="container">
    <div class="slider">
      <!--  -->
      <div class="img-container">
        <img src="../assets/slider0.1.png" class="img-slider" alt />
      </div>
      <!--  -->
      <div class="titles-container">
        <img src="../assets/icon1.svg" class="icon1" />
        <h1 class="title1">Junta de vecinos ciudad real II</h1>
        <h1 class="title2">EL MEJOR LUGAR PARA VIVIR CON TU FAMILIA</h1>
        <img src="../assets/icon2.svg" class="icon2" />
      </div>
      <!--  -->
    </div>
    <img src="https://imgur.com/6Dkiz9q" alt />
  </div>
</template>
<script>
export default {
  name: "slider"
};
</script>
<style scoped>
@import url("https://fonts.googleapis.com/css?family=Playball|Rosarivo&display=swap");

.slider {
  position: relative;
}
.img-slider {
  height: 1024px;
  width: 100%;
}
.titles-container {
  align-items: center;
  justify-content: center;
  text-align: center;
  margin: 200px 400px 600px 0px;
  position: absolute;
  width: 100%;
  /* left: 10px 10px 10px; */
  z-index: 2;
}
.img-container {
  position: absolute;
  width: 100%;
  z-index: 1;
}

.title1 {
  font-family: "Playball", cursive;
  color: white;
  font-size: 60px;
  font-weight: 100;
  margin: 10px;
}
.title2 {
  font-family: "Rosarivo", serif;
  color: white;
  font-size: 35px;
  font-weight: 100;
  margin: 10px;
}
.icon1 {
  margin: 30px;
}
.icon2 {
  margin: 15px 0px 0px 0px;
}
</style>