<template>
  <div class="container">
    <nav class="menu">
      <!-- ---------------------------------------------- -->
      <div class="logo-name">
        <div class="background-image">
          <img src="../../assets/ciudad real.png" class="img" />
        </div>
        <p>ciudad real</p>
      </div>
      <!-- ---------------------------------------------- -->
      <div class="list-container">
        <div class="list" v-for="list in title" :key="list.id">
          <ul>
            <li>
              <a href>{{list.label}}</a>
            </li>
          </ul>
        </div>
      </div>
      <!-- ---------------------------------------------- -->
      <div class="user">
        <img src="../../assets/user.svg" class="img-user" />
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "sidebar",
  data() {
    return {
      title: [
        { id: 1, label: "Inicio" },
        { id: 2, label: "Comunicados" },
        { id: 3, label: "Noticias" },
        { id: 4, label: "Actividades" },
        { id: 5, label: "Revista" },
        { id: 5, label: "Transparencia" },
        { id: 5, label: "Sobre nosotros" },
        { id: 5, label: "Contactanos" }
      ]
    };
  }
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Playball|Roboto:300|Rosarivo&display=swap");
* {
  font-family: "Roboto", sans-serif;
  color: #d2a35c;
  font-weight: 200;
  font-size: 18px;
}
.container {
  width: 100%;
}
.menu {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 70px;
  /* border: 1px solid red;
  background-color: black; */
}
.logo-name {
  height: 100%;
  width: 200px;
  display: flex;
  justify-content: center;
  align-items: center;
  /* border: 1px solid red; */
}
.background-image {
  height: 56px;
  width: 56px;
  background-color: #f3debf;
  border-radius: 50%;
  margin: 10px;
  /* border: 1px solid red; */
  display: flex;
  justify-content: center;
  align-items: center;
}
.img {
  height: 45px;
  width: 45px;
}
.list ul,
a {
  list-style: none;
  text-decoration: none;
  margin: 0px;
  /* padding: 0px; */
}
.list ul li a {
  padding: 25px 15px 19px 15px;
  border-bottom: 5px solid rgba(174, 139, 89, 50%);
}

.list ul li a:hover {
  background-color: rgba(174, 139, 89, 50%);
  color: #ae8b59;
  border-bottom: 5px solid rgba(174, 139, 89);
  transition-duration: 1s, 1s;
}

.list {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
}
.list-container {
  width: 50%;
  margin-right: 35%;
  display: flex;
}
.user {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-right: 20px;
  height: 50%;
  width: 35px;
  background-color: #f3debf;
  border-radius: 50%;
}
</style>