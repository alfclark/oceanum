<template>
  <footer class="footer">
    <img class="footer_logo" src="@/assets/logo.svg" alt="logo" />
    <div class="social">
      <a href="" target="”_blank”"><i class="fa-brands fa-facebook-f"></i></a>
      <a href="" target="”_blank”"><i class="fa-brands fa-linkedin-in"></i></a>
      <a href="" target="”_blank”"><i class="fa-brands fa-instagram"></i></a>
      <a href="" target="”_blank”"><i class="fa-brands fa-twitter"></i></a>
      <a href="" target="”_blank”"><i class="fa-brands fa-tiktok"></i></a>
    </div>
    <div class="credits">
      <h2 class="by_us">2022 <span>©</span> Hecho con amor al mar, Oceanum.</h2>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterView",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.footer {
  height: 100%;
  background-color: var(--water);
  display: flex;
  flex-direction: column;
}

.footer_logo {
  height: 80px;
  width: 80px;
  position: absolute;
  transform: translate(-50%, -50%);
  left: 50%;
}
.social {
  margin-top: 4rem;
  position: relative;
  display: flex;
  gap: 1rem;
  justify-content: center;
}
.fa-brands {
  font-size: 1.2rem;
  color: white;
}
.fa-brands:hover {
  color: var(--orange);
  transition: 0.4s;
}

.by_us {
  text-align: center;
  color: rgba(255, 255, 255, 0.863);
  font-weight: 500;
  font-size: 0.7rem;
  margin-top: 1rem;
  padding-bottom: 1rem;
  text-decoration: none;
}
</style>
