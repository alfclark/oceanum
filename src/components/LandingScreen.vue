<template>
  <div id="landing" class="landing">
    <section class="hero">
      <div class="hero-left">
        <h2 class="slogan">Nosotros y el mar</h2>
        <div class="brand-name">
          <h1 class="brand">OCEANUM</h1>
          <h2 class="dot">.</h2>
        </div>

        <h2>Desarrollamos éste proyecto con una sola finalidad:</h2>
        <h3>Preservar la vida en nuestros mares.</h3>
      </div>
      <div class="hero-right"></div>
    </section>
  </div>
</template>

<script>
export default {};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.landing {
  height: 90vh;
  display: flex;
  flex-direction: column;
  align-content: center;
  justify-content: center;
  position: static;
}
.hero {
  position: relative;
  height: 100%;
  padding-top: 3rem;
  color: var(--carbon);
  display: flex;
}
.slogan {
  font-size: 1rem;
}
.brand.name {
}
</style>
