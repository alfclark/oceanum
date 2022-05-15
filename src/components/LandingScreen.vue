<template>
  <div id="landing" class="landing">
    <section class="hero">
      <div class="hero-left">
        <h2 class="slogan">Nosotros y el mar</h2>
        <div class="brand-name">
          <h1 class="brand">OCEANUM</h1>
          <h1 class="dot">.</h1>
        </div>
        <h2 class="sub">Desarrollamos éste proyecto con una sola finalidad:</h2>
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
  position: static;
}
.hero {
  position: relative;
  height: 100%;
  padding-top: 3rem;
  color: var(--carbon);
  display: flex;
}
.hero-left {
  padding-left: 2rem;
  display: flex;
  flex-direction: column;
  justify-content: left;
  align-items: flex-start;
}
.slogan {
  font-size: 1rem;
}
.brand-name {
  display: flex;
}
.brand-name h1 {
  font-size: 3rem;
}
.brand {
  letter-spacing: 5px;
}
.dot {
  color: var(--water);
}
.sub {
  font-size: 1rem;
}
</style>
