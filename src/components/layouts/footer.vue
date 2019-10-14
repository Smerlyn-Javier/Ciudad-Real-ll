<template>
  <div class="container">
    <footer class="footer">
      <div class="footer-container">
        <div class="container-logo-submenu">
          <div class="logo">
            <img src="../../assets/ciudad real.png" class="img-logo" />
          </div>
          <!--  -->
          <div class="submenu">
            <ul>
              <li v-for="list in title.slice(0,5)" :key="list.id">
                <a href>{{list.label}}</a>
              </li>
            </ul>
            <ul>
              <li v-for="list in title.slice(5,8)" :key="list.id">
                <a href>{{list.label}}</a>
              </li>
            </ul>
          </div>
          <!--  -->
        </div>
        <div class="contacts">
          <h1>Contactos</h1>
          <h2>Correo: Example@gmail.com</h2>
          <h2>Telefono: 809-XXX-XXX</h2>
          <h2>Direccion: C/example 34 B/Example</h2>

          <div class="redes">
            <img src="../../assets/twitter.svg" class="instagram" />
            <img src="../../assets/instagram.svg" class="twitter" />
          </div>
        </div>
      </div>
      <div class="copyright">
        <h1>
          © Copyright 2015 - Junta de Vecinos Ciudad Real II - Nombre y marca registrada
          en ONAPI y Cámara de Comercio de la República Dominicana.
        </h1>
      </div>
    </footer>
  </div>
</template>
<script>
export default {
  name: "footer",
  data() {
    return {
      title: [
        { id: 1, label: "Inicio" },
        { id: 2, label: "Comunicados" },
        { id: 3, label: "Noticias" },
        { id: 4, label: "Actividades" },
        { id: 5, label: "Revista" },
        { id: 6, label: "Transparencia" },
        { id: 7, label: "Sobre nosotros" },
        { id: 8, label: "Contactanos" }
      ]
    };
  }
};
</script>
<style scoped>
@import url("https://fonts.googleapis.com/css?family=Playball|Roboto:300|Rosarivo&display=swap");
* {
  color: white;
}
.footer {
  height: 10%;
  background-color: #d4b485;
}
.footer-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 200px;
  background-color: #d4b485;
}
.logo {
  display: flex;
  justify-content: center;
  align-items: center;
  /* border: 1px solid red; */
  height: 150px;
  width: 150px;
  margin: 20px;
  border-radius: 150px;
  background-color: #f3debf;
}
.img-logo {
  height: 100px;
  width: 100px;
}
.submenu {
  display: flex;
  /* border: 1px solid red; */
  height: 150px;
  width: 350px;
  margin: 20px;
}
.submenu ul li a {
  font-family: Roboto;
  text-decoration: none;
  margin: 10px;
}
.submenu ul li {
  margin: 10px;
}
.submenu ul {
  margin: 5px;
}
.contacts {
  /* border: 1px solid red; */
  height: 150px;
  width: 500px;
  margin: 20px;
}
.contacts h1 {
  font-weight: bold;
  font-size: 25px;
  font-family: "Roboto", serif;
}
.contacts h2 {
  font-weight: 300;
  font-size: 15px;
  margin: 10px;
  font-family: "Rosarivo", serif;
}
.redes {
  display: flex;
  justify-content: center;
  align-items: center;
}
.redes img {
  margin: 10px;
}
.copyright {
  height: 60px;
  font-size: 8px;
  font-family: "Rosarivo", serif;
}

.copyright h1 {
  margin: 20px;
  width: 700px;
}

.container-logo-submenu {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>