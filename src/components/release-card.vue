<template>
  <div class="container">
    <div class="card1">
      <img src="../assets/family.svg" alt />
    </div>
    <div class="card2">
      <div class="iconContainer">
        <img src="../assets/icon3.svg" class="icon-edi" />
      </div>
      <div class="card2Container">
        <h1>Junta de vecinos ciudad real II</h1>
        <h2>Comunicados</h2>
        <h3>
          Nos apasiona el servicio
          y el trabajo desprendido
          hacia los demás, perseguimos
          con entusiasmo las buenas
          costumbres, educando a nuestros
          jóvenes y adultos e induciéndolos
          a unirse en protección de su
          comunidad. Te invitamos a ser
          parte activa de nuestra comunidad,
          modelando
        </h3>
        <div class="button">click aca</div>
      </div>
    </div>
    <div class="card3">
      <img src="../assets/edi.svg" alt />
    </div>
  </div>
</template>
<script>
export default {
  name: "release-card"
};
</script>
<style scoped>
@import url("https://fonts.googleapis.com/css?family=Playball|Roboto:300|Rosarivo&display=swap");
.card1 {
  width: 33.33%;
  height: 626px;
  border: red solid 1px;
  background-color: rgba(174, 139, 89, 50%);
}
.card1 img {
  height: 100%;
  width: 100%;
  /* opacity: 0.9; */
  object-fit: cover;
}
.card2 {
  width: 33.33%;
  height: 626px;
  background-color: #ae8b59;
  border: red solid 1px;
  /* display: flex;
  justify-content: center;
  align-content: center; */
}
.card2Container {
  width: 50%;
  margin: 0 auto;
}
.card2 h1 {
  font-family: "Playball", sans-serif;
  margin: 0 auto;
}
.card2 h2 {
  font-family: "Rosarivo", sans-serif;
  margin: 0 auto;
}
.card2 h3 {
  margin: 10px;
  text-align: center;
  font-family: "Rosarivo", sans-serif;
}
.iconContainer {
  display: flex;
  justify-content: center;
  align-content: center;
}
.icon-edi {
  margin: 20px;
}
.card3 {
  width: 33.33%;
  height: 626px;
  border: red solid 1px;
}
.card3 img {
  height: 100%;
  width: 100%;
  object-fit: cover;
}
.container {
  width: 100%;
  display: flex;
}
.button {
  background-color: #d4b485;
  font-size: 20px;
  color: white;
  margin: 0 auto;
  margin-top: 25%;
  width: 200px;
  height: 50px;
  border-radius: 10px;
  justify-content: center;
  align-items: center;
  display: flex;
}
</style>