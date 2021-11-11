<template>
  <Navbar />
  <Home />
  <About />
  <Creations />
  <Footer />
</template>

<script>
import About from "./components/About.vue";
import Creations from "./components/Creations.vue";
import Footer from "./components/Footer.vue";
import Home from "./components/Home.vue";
import Navbar from "./components/Navbar.vue";

export default {
  name: "App",
  components: {
    Navbar,
    Home,
    About,
    Creations,
    Footer,
  },
};
</script>

<style>
:rot {
  --desktop: 375px;
  --Desktop: 1440px;

  --White: hsl(0, 0%, 100%);
  --Black: hsl(0, 0%, 0%);
  --Dark-Gray: hsl(0, 0%, 55%);
  --Very-Dark-Gray: hsl(0, 0%, 41%);
}
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}
html {
  scroll-behavior: smooth;
}
body {
  font-family: "Alata", sans-serif;
}
.subtitle {
  font-family: "Josefin Sans", sans-serif;
  font-size: 2.6em;
  font-weight: 300;
  text-transform: uppercase;
  margin: 1.4em 0 0.45em;
  max-width: 350px;
}

.center,
#about,
#creations {
  width: 700px;
  margin: auto;
}
.center {
  display: flex;
  justify-content: start;
  align-items: center;
  flex-direction: column;
  margin: auto;
  padding: 28px;
}
@media (min-width: 1400px) {
  .center {
    width: 1340px;
    flex-direction: row;
  }
  #navbar {
    padding-top: 4em;
    padding-left: calc(10em + 28px);
    padding-right: calc(10em + 28px);
  }
  .navbar__title {
    font-size: 2.9em;
  }
  .navbar__hamburguese {
    display: none;
  }
  .navbar__menu {
    display: flex;
    align-items: center;
    justify-content: center;
    column-gap: 40px;
    color: #fff;
  }

  #home {
    min-height: 90vh;
    background-image: url(./assets/desktop/image-hero.jpg);
    justify-content: start;
  }
  .home__container {
    padding: 50px;
  }
  .home__container__title {
    font-size: 5.2em;
    max-width: 8.7em;
  }

  #about {
    text-align: start;
    width: 1340px;
    flex-direction: row;
  }
  .about__container {
    align-self: flex-end;
    padding: 110px 0 0 110px;
    margin-left: -220px;
    background-color: #fff;
    max-width: 637px;
  }
  #about .subtitle {
    font-size: 3.2em;
    margin: 0 0 35px 0;
    max-width: none;
  }
  .about__info {
    max-width: none;
    line-height: 33px;
  }
  .about__img {
    width: 940px;
  }

  #creations {
    width: 1340px;
    display: grid;
    grid-template-columns: repeat(4, 300px);
  }
  #creations .subtitle {
    font-size: 3.2em;
    grid-column: span 3;
    margin-bottom: 50px;
    max-width: 440px;
  }
  .creations__btn {
    grid-row: 1;
    grid-column: 4/5;
  }
  .creations__creation {
    height: 500px;
  }
  .creations__creation__subtitle {
    margin: 0 40px 40px;
    font-size: 2.5em;
    max-width: none;
  }
  .creations__creation:nth-child(2) {
    background-image: url(./assets/desktop/image-deep-earth.jpg);
  }
  .creations__creation:nth-child(3) {
    background-image: url(./assets/desktop/image-night-arcade.jpg);
  }
  .creations__creation:nth-child(4) {
    background-image: url(./assets/desktop/image-soccer-team.jpg);
  }
  .creations__creation:nth-child(5) {
    background-image: url(./assets/desktop/image-grid.jpg);
  }
  .creations__creation:nth-child(6) {
    background-image: url(./assets/desktop/image-from-above.jpg);
  }
  .creations__creation:nth-child(7) {
    background-image: url(./assets/desktop/image-pocket-borealis.jpg);
  }
  .creations__creation:nth-child(8) {
    background-image: url(./assets/desktop/image-curiosity.jpg);
  }
  .creations__creation:nth-child(9) {
    background-image: url(./assets/desktop/image-fisheye.jpg);
  }

  #footer .center {
    display: grid;
    grid-template-columns: 1fr 1fr;
  }
  .footer__social {
    grid-row: 1;
    grid-column: 2/3;
    justify-content: end;
  }
  .footer__about {
    flex-direction: row;
    justify-content: start;
    column-gap: 25px;
  }
  .footer__copyright {
    font-size: 1.2em;
    text-align: end;
  }
}
@media (max-width: 450px) {
  .home__container__title {
    font-size: 2em;
  }
  .subtitle {
    font-size: 2em;
  }
  .creations__creation__subtitle {
    font-size: 1.8em;
  }
}
</style>
