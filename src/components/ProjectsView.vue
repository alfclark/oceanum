<template>
  <!-- Skills Section -->
  <div style="margin-top: -50px; position: absolute" id="skills"></div>
  <section class="container">
    <div class="proyectos">
      <h1 class="subtitle">
        Proyectos:
        <hr class="divider" />
      </h1>
      <div class="proyectos-wrapper">
        <a href="" class="proyecto">
          <img src="" alt="" class="logo" />
          <h2 class="title"></h2>
          <p class="desc"></p>
        </a>
      </div>
    </div>
  </section>
</template>

<script></script>

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
}

@media screen and (max-width: 900px) {
  .skills-wrapper {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
    padding: 0;
  }
}
</style>
