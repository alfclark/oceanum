<template>
  <div style="margin-top: -100px; position: absolute" id="about"></div>
  <section class="container">
    <div class="about-us">
      <h1 class="subtitle">
        Nosotros:
        <hr class="divider" />
      </h1>
      <p class="desc">
        Oceanum significa "Océano" en Latín. Un día, algo que inició como una
        simple idea para competir en un hackathon, nos ayudó a darnos cuenta de
        la gran desinformación que existe en la gente, en lo que respecta a la
        contaminación del océano y las especies que están en peligro de
        extinción que habitan en ellos. Por lo cual, sumamos esfuerzos y
        conocimientos para desarrollar una herramienta, que ayude a las personas
        a conocer más acerca de los mares y océanos Mexicanos, las especies que
        viven ellos, y los problemas que enfrentan esos ecosistemas. A su vez,
        presentamos ante la gente, a distintas asociaciones que trabajan
        arduamente en la preservación de los océanos y sus especies, para que
        también el público en general pueda sumarse al apoyo de estas grandes
        causas. Ya sea con voluntariado o de forma económica.
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
  flex-direction: column;
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
