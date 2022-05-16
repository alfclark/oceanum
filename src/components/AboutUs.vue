<template>
  <div style="margin-top: -50px; position: absolute" id="about"></div>
  <section class="container">
    <div class="about-us">
      <h1 class="subtitle">
        Nosotros:
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
.about-us {
  width: 70vw;
  text-align: center;
}
@media screen and (max-width: 550px) {
  .about-us {
    width: 90vw;
  }
}
</style>
