<template>
  <nav id="navbar">
    <h2 class="navbar__title">Loopstudios</h2>
    <ul class="navbar__menu" @click="navMenu">
      <li><a class="a" href="#about">About</a></li>
      <li><a class="a" href="#creations">Careers</a></li>
      <li><a class="a" href="#footer">Events</a></li>
      <li><a class="a" href="#footer">Products</a></li>
      <li><a class="a" href="#footer">Support</a></li>
    </ul>
    <div class="navbar__hamburguese" @click="navMenu"></div>
  </nav>
</template>

<script>
export default {
  setup() {
    const navMenu = (e) => {
      const menu = document.querySelector(".navbar__menu");
      if (e.target.className == "a") menu.classList.remove("toggleMenu");
      else if (e.target.className == "navbar__hamburguese") {
        menu.classList.toggle("toggleMenu");
      }
    };

    return { navMenu };
  },
};
</script>

<style>
#navbar {
  width: 100%;
  position: absolute;
  top: 0;
  left: 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 40px 28px;
  color: #fff;
}
.navbar__title {
  position: relative;
  font-size: 2.2em;
  letter-spacing: 1px;
  z-index: 11;
}
.navbar__menu {
  display: none;
}
.navbar__hamburguese {
  cursor: pointer;
  background-image: url(../assets/icon-hamburger.svg);
  background-size: cover;
  width: 32px;
  height: 22px;
}
.navbar__menu li {
  list-style: none;
}
.navbar__menu a {
  font-size: 20px;
  color: #fff;
  text-decoration: none;
}

.toggleMenu {
  display: flex;
  align-items: start;
  justify-content: center;
  flex-direction: column;
  position: absolute;
  inset: 0;
  padding-left: 28px;
  width: 100%;
  height: 100vh;
  background-color: #000;
  row-gap: 35px;
}
.toggleMenu a {
  font-size: 2.8em;
  font-family: "Josefin Sans", sans-serif;
  font-weight: 300;
}
.navbar__hamburguese {
  position: relative;
  z-index: 11;
}
.toggleMenu ~ .navbar__hamburguese {
  background-image: url(../assets/icon-close.svg);
  height: 32px;
}
</style>
