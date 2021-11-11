<template>
  <main id="home">
    <div class="center">
      <div class="home__container">
        <h1 class="home__container__title">Immersive experiences that deliver</h1>
      </div>
    </div>
  </main>
</template>

<script>
export default {};
</script>

<style>
#home {
  min-height: 84vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background-image: url(../assets/mobile/image-hero.jpg);
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
  color: #fff;
  padding: 0 28px;
  background-color: #00000052;
  background-blend-mode: soft-light;
}
.home__container {
  padding: 30px 28px;
  border: 3px solid #fff;
}
.home__container__title {
  font-size: 2.85em;
  font-weight: 300;
  font-family: "Josefin Sans", sans-serif;
  letter-spacing: 3px;
  text-transform: uppercase;
  max-width: 365px;
}
</style>
