<template>
  <!-- Skills Section -->
  <div style="margin-top: -50px; position: absolute" id="projects"></div>
  <section class="container">
    <div class="proyectos">
      <h1 class="subtitle">
        Proyectos:
        <hr class="divider" />
      </h1>
      <p class="desc">
        Sé parte del cambio, presentamos los proyectos vigentes para la
        protección y cuidado de nuestras costas y océanos.
      </p>
      <div class="proyectos-wrapper">
        <div class="proyecto">
          <div class="org-logo">
            <img
              src="https://assets01.teamassets.net/assets/images/teamseas-tm-logo.png"
              alt=""
              class="logo"
            />
          </div>
          <div class="prog-title">
            <h1 class="programa">#TeamSeas</h1>
          </div>
          <div class="prog-desc">
            <p class="desc-text">
              Limpieza del Océano. 1 Dólar donado = 1 libra de basura que se
              limpia.
            </p>
          </div>
          <a class="donar" href="https://teamseas.org/" target="”_blank”"
            >Donar</a
          >
        </div>
        <div class="proyecto">
          <div class="org-logo">
            <img
              src="https://earthleagueinternational.org/wp-content/uploads/2020/04/earth-league-international.png"
              alt=""
              class="logo"
            />
          </div>
          <div class="prog-title">
            <h1 class="programa">Operación Fake Gold</h1>
          </div>
          <div class="prog-desc">
            <p class="desc-text">
              Detener la cadena de suministro ilegal de Totoaba de México a
              China
            </p>
          </div>
          <a
            class="donar"
            href="https://earthleagueinternational.org/donate/"
            target="”_blank”"
            >Donar</a
          >
        </div>
        <div class="proyecto">
          <div class="org-logo">
            <img
              src="http://www.seiche.com/wp-content/uploads/2018/06/Ocean-CleanUp-portrait-blue.png"
              alt=""
              class="logo"
            />
          </div>
          <div class="prog-title">
            <h1 class="programa">The Ocean Clean Up</h1>
          </div>
          <div class="prog-desc">
            <p class="desc-text">
              Limpieza del Océano mediante el diseño de tecnología y actividades
              de limpieza.
            </p>
          </div>
          <a
            class="donar"
            href="https://theoceancleanup.com/donate/"
            target="”_blank”"
            >Donar</a
          >
        </div>
        <div class="proyecto">
          <div class="org-logo">
            <img
              src="https://mx.oceana.org/wp-content/uploads/sites/17/logo_es-e1631518823246.png"
              alt=""
              class="logo"
            />
          </div>
          <div class="prog-title">
            <h1 class="programa">Proyecto Alacranes</h1>
          </div>
          <div class="prog-desc">
            <p class="desc-text">
              Protegiendo los hábitats marinos de las costas de México contra
              pesca furtiva y contaminación.
            </p>
          </div>
          <a
            class="donar"
            href="https://oceana.ca/en/donate-oceana-canada/"
            target="”_blank”"
            >Donar</a
          >
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import axios from "axios";
export default {
  data: () => ({
    result: null
  }),
  created() {
    axios.get("https://jsonplaceholder.typicode.com/todos/1").then((result) => {
      this.result = result.data;
      //
    })
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container {
  width: 90vw;
  display: flex;
  align-items: center;
  justify-content: center;
}
.subtitle {
  color: var(--carbon);
}
.desc {
  color: var(--carbon);
}
.proyectos {
  width: 70vw;
  margin: 4rem 0;
  text-align: center;
}
.proyectos-wrapper {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
  gap: 2rem;
}
.proyecto {
  display: flex;
  flex-direction: column;
  background-color: var(--water);
  align-items: center;
  padding: 1.5rem;
  width: 12rem;
  height: 25rem;
  border-radius: 1rem;
}
.org-logo {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 30%;
  background-color: white;
  padding: 10px;
}
.logo {
  width: 9rem;
}
.prog-title {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 20%;
  padding-top: 1rem;
}
.programa {
  font-size: 1.2rem;
}
.prog-desc {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 40%;
}
.desc-text {
  font-size: 0.9rem;
}
.donar {
  background-color: var(--orange);
  position: relative;
  text-decoration: none;
  color: white;
  font-size: 1.2rem;
  padding: 0.3rem 1.2rem;
  border-radius: 1.5rem;
  bottom: 0;
}
.donar:hover {
  background-color: var(--sunshine);
  transition: 0.4s;
}

@media screen and (max-width: 550px) {
  .proyectos {
    width: 90vw;
  }
  .proyectos-wrapper {
    gap: 1rem;
  }
  .proyecto {
    display: flex;
    flex-direction: column;
    background-color: var(--water);
    align-items: center;
    justify-content: center;
    gap: 1rem;
    padding: 1rem;
    width: 9rem;
    border-radius: 1rem;
  }
  .logo {
    width: 6rem;
  }
  .programa {
    font-size: 1rem;
  }
}
</style>
