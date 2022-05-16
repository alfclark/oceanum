<template>
  <div id="landing" class="landing">
    <section class="hero">
      <h2 class="slogan">Nosotros y el mar</h2>
      <img src="@/assets/logo.svg" alt="" class="logo" />
      <div class="brand-name">
        <h1 class="brand">OCEANUM</h1>
        <h1 class="dot">.</h1>
      </div>
      <div class="desc">
        <h2 class="sub">Desarrollamos éste proyecto con una sola finalidad:</h2>
        <h3>Preservar la vida en nuestros mares.</h3>
      </div>
    </section>
    <div class="scroll-me">
      <p class="scroll-text">Sigue descubriendo</p>
      <i class="fa-solid fa-arrow-down"></i>
    </div>
    <div class="custom-shape-divider-bottom-1652672471">
      <svg
        data-name="Layer 1"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 1200 120"
        preserveAspectRatio="none"
      >
        <path
          d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V0H0V27.35A600.21,600.21,0,0,0,321.39,56.44Z"
          class="shape-fill"
        ></path>
      </svg>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.landing {
  height: 100vh;
  display: flex;
  flex-direction: column;
  position: static;
}
.hero {
  position: relative;
  padding: 3rem;
  color: var(--carbon);
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 3rem;
  gap: 0.5rem;
}
.logo {
  width: 15rem;
  border: solid 2px var(--water);
  border-radius: 50%;
}
.slogan {
  font-size: 1.2rem;
  letter-spacing: 2px;
  text-decoration: underline;
}
.brand-name {
  display: flex;
}

.brand {
  font-size: 3rem;
  letter-spacing: 10px;
}
.dot {
  padding-left: 1rem;
  color: var(--water);
  font-size: 3rem;
}
.desc {
  margin-top: 1rem;
}
.sub {
  font-size: 1rem;
}
.scroll-me {
  color: var(--carbon);
  font-size: 0.9rem;
  text-align: center;
  justify-content: center;
  animation: bounce1 2s infinite, show1 5s forwards;
  position: absolute;
  bottom: 0;
  width: 100%;
}
.scroll-text {
  margin: 0;
}

@media screen and (max-width: 500px) {
  .logo {
    width: 10rem;
  }
  .scroll-me {
    font-size: 0.7rem;
  }
}
</style>
