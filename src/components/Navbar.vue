<template>
  <div class="navbar">
    <nav
      id="navContainer"
      class="navbar sticky-top navbar-expand-lg navbar-dark"
    >
      <button
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav mx-auto">
          <li class="nav-item">
            <router-link to="/" class="nav-link">
              Inicio
            </router-link>
          </li>
          <li class="nav-item">
            <router-link to="/tablacontenido" class="nav-link"
              >Tabla de Contenido</router-link
            >
          </li>
          <li class="nav-item">
            <router-link to="/proposito" class="nav-link"
              >Propósito</router-link
            >
          </li>
          <li class="nav-item">
            <router-link to="/desarrollo" class="nav-link"
              >Desarrollo del Tema</router-link
            >
          </li>
          <li class="nav-item">
            <router-link to="/conclusiones" class="nav-link"
              >Conclusiones</router-link
            >
          </li>
          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              id="navbarDropdownMenuLink"
              data-toggle="dropdown"
              aria-haspopup="true"
              aria-expanded="false"
              >Mas..</a
            >
            <div class="dropdown-menu" aria-labelledby="navbarDropdownMenuLink">
              <router-link to="/referentes" class="dropdown-item"
                >Referentes Bibliográficos</router-link
              >
              <router-link to="/creditos" class="dropdown-item" href="#"
                >Créditos</router-link
              >
            </div>
          </li>
        </ul>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.navbar {
  width: 100%;
}
#navContainer {
  background-color: rgb(14, 48, 97);
  margin-left: 4.3%;
  margin-right: 4.3%;
}
ul {
  /* background-color: blueviolet; */
  font-size: 23px;
}
li {
  padding-left: 10px;
  padding-right: 10px;
  font-weight: 550;
}
.dropdown-menu {
  left: auto;
  right: 0;
  font-size: 27px;
}
</style>
