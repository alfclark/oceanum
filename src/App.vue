<template>
  <NavBar />
  <LandingScreen />
  <MapView />
  <SkillsView />
  <GoTop />
  <AboutUs />
  <ContactSection />
  <FooterView />
</template>

<script>
import NavBar from "./components/NavBar.vue";
import LandingScreen from "./components/LandingScreen.vue";
import AboutUs from "./components/AboutUs.vue";
import SkillsView from "./components/ProjectsView.vue";
import FooterView from "./components/FooterView.vue";
import GoTop from "./components/GoTop.vue";
import ContactSection from "./components/ContactSection.vue";
import MapView from "./components/MapView.vue";

export default {
  name: "App",
  components: {
    NavBar,
    LandingScreen,
    AboutUs,
    FooterView,
    SkillsView,
    GoTop,
    ContactSection,
    MapView,
  },
};
</script>

<style>
/* CUSTOM SCROLLBAR */
::-webkit-scrollbar-track {
  background-color: #141c3a1a;
}

::-webkit-scrollbar {
  width: 12px;
  background-color: var(--dark);
}

::-webkit-scrollbar-thumb {
  background-color: var(--water);
}
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
:root {
  --water: #0099ff;
  --waterDark: #1f3a4d;
  --sunshine: #ffb72b;
  --sand: #ffdb59;
  --orange: #ff9900;
  --orangeDark: #c28b39;
  --black: #23221a;
  --carbon: #292929;
}
/* ANIMATIONS */
@keyframes bounce1 {
  0% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-20px);
  }
  100% {
    transform: translateY(0);
  }
}
@keyframes entrance1 {
  0% {
    animation-timing-function: ease-in;
    opacity: 0;
    transform: translateY(-250px);
  }

  38% {
    animation-timing-function: ease-out;
    opacity: 1;
    transform: translateY(0);
  }

  55% {
    animation-timing-function: ease-in;
    transform: translateY(-65px);
  }

  72% {
    animation-timing-function: ease-out;
    transform: translateY(0);
  }

  81% {
    animation-timing-function: ease-in;
    transform: translateY(-28px);
  }

  90% {
    animation-timing-function: ease-out;
    transform: translateY(0);
  }

  95% {
    animation-timing-function: ease-in;
    transform: translateY(-8px);
  }

  100% {
    animation-timing-function: ease-out;
    transform: translateY(0);
  }
}
@keyframes show1 {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@keyframes shake1 {
  0%,
  100% {
    transform: translateX(0);
  }

  10%,
  30%,
  50%,
  70% {
    transform: translateX(-2px);
  }

  20%,
  40%,
  60% {
    transform: translateX(2px);
  }

  80% {
    transform: translateX(1px);
  }

  90% {
    transform: translateX(-1px);
  }
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  color: white;
  text-align: center;
  background-color: var(--sand);
}
.custom-shape-divider-bottom-1652672471 {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  overflow: hidden;
  line-height: 0;
  transform: rotate(180deg);
}

.custom-shape-divider-bottom-1652672471 svg {
  position: relative;
  display: block;
  width: calc(100% + 1.3px);
  height: 100%;
}

.custom-shape-divider-bottom-1652672471 .shape-fill {
  fill: #0099ff;
}
</style>
