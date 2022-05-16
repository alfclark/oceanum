<template>
  <nav class="navbar sticky-top navbar-expand-lg navbar-dark">
    <div class="container-fluid">
      <a href="#" class="logo">
        <img class="navbar-brand" src="@/assets/fish.png" alt="logo" />
      </a>

      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link" href="#map">Mapa</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#projects">Proyectos</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#about">Nosotros</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#contact"
              ><button class="nav-button">Contáctanos</button></a
            >
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "NavBar",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.navbar {
  background-color: var(--water);
  padding: 0.5rem 2rem;
  box-shadow: 0 0 20px var(--water);
}
.logo {
  display: flex;
  flex-direction: column;
  align-content: center;
  align-items: center;
  justify-content: center;
  color: #fff;
  cursor: pointer;
  text-decoration: none;
}
.navbar-brand {
  width: 50px;
  margin: 0;
}

.navbar-nav {
  align-items: center;
}
.nav-link {
  color: white;
  font-weight: 500;
  font-size: 1rem;
  margin: 0 0.5rem;
}
.nav-button {
  text-decoration: none;
  color: #fff;
  font-size: 1rem;
  padding: 0.5rem 1.5rem;
  background-color: transparent;
  border: none;
  border: solid;
  border-radius: 2.2rem;
}
.nav-button:hover {
  background-color: var(--waterDark);
  transition: 0.4s;
}
</style>
