<template>
  <div style="margin-top: -100px; position: absolute" id="map"></div>
  <section class="container">
    <div class="map">
      <h1 class="subtitle">
        Mapa Interactivo:
        <hr class="divider" />
      </h1>
      <p class="desc">
        Conoce en qué zonas se encuentran algunas de las especies en peligro.
      </p>
    </div>
  </section>
</template>

<script>
export default {};
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
.map {
  width: 70vw;
  text-align: center;
}
@media screen and (max-width: 550px) {
  .map {
    width: 90vw;
  }
}
</style>
