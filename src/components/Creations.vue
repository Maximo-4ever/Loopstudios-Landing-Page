<template>
  <article id="creations">
    <h3 class="subtitle">Our Creations</h3>
    <section class="creations__creation">
      <h4 class="creations__creation__subtitle">Deep earth</h4>
    </section>
    <section class="creations__creation">
      <h4 class="creations__creation__subtitle">Night arcade</h4>
    </section>
    <section class="creations__creation">
      <h4 class="creations__creation__subtitle">Soccer team vr</h4>
    </section>
    <section class="creations__creation">
      <h4 class="creations__creation__subtitle">The grid</h4>
    </section>
    <section class="creations__creation">
      <h4 class="creations__creation__subtitle">From up above vr</h4>
    </section>
    <section class="creations__creation">
      <h4 class="creations__creation__subtitle">Pocket borealis</h4>
    </section>
    <section class="creations__creation">
      <h4 class="creations__creation__subtitle">The curiosity</h4>
    </section>
    <section class="creations__creation">
      <h4 class="creations__creation__subtitle">Make it fisheye</h4>
    </section>
    <button class="creations__btn">See all</button>
  </article>
</template>

<script>
export default {};
</script>

<style>
#creations {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  padding: 28px;
  gap: 30px;
}
.creations__creation {
  position: relative;
  width: 100%;
  height: 158px;
  display: flex;
  flex-direction: column-reverse;
  background-size: cover;
  background-blend-mode: soft-light;
  cursor: pointer;
}
.creations__creation::after {
  content: "";
  position: absolute;
  inset: 1;
  width: 100%;
  height: 100%;
  background: radial-gradient(
    circle,
    rgba(255, 255, 255, 0) 32%,
    rgba(0, 0, 0, 0.7959558823529411) 100%
  );
  z-index: 11;
  transition: 0.2s;
}
.creations__creation:hover::after {
  background: rgba(255, 255, 255, 0.62);
}
.creations__creation:hover .creations__creation__subtitle {
  color: #000;
}
.creations__creation:nth-child(2) {
  background-image: url(../assets/mobile/image-deep-earth.jpg);
}
.creations__creation:nth-child(3) {
  background-image: url(../assets/mobile/image-night-arcade.jpg);
}
.creations__creation:nth-child(4) {
  background-image: url(../assets/mobile/image-soccer-team.jpg);
}
.creations__creation:nth-child(5) {
  background-image: url(../assets/mobile/image-grid.jpg);
}
.creations__creation:nth-child(6) {
  background-image: url(../assets/mobile/image-from-above.jpg);
}
.creations__creation:nth-child(7) {
  background-image: url(../assets/mobile/image-pocket-borealis.jpg);
}
.creations__creation:nth-child(8) {
  background-image: url(../assets/mobile/image-curiosity.jpg);
}
.creations__creation:nth-child(9) {
  background-image: url(../assets/mobile/image-fisheye.jpg);
}
.creations__creation__subtitle {
  max-width: 180px;
  font-family: "Josefin Sans", sans-serif;
  font-size: 2em;
  font-weight: 300;
  text-transform: uppercase;
  margin: 0 24px 24px;
  color: #fff;
  z-index: 111;
}
.creations__btn {
  margin-top: 25px;
  text-transform: uppercase;
  font-weight: 200;
  font-size: 1.2em;
  letter-spacing: 6px;
  padding: 15px 40px;
  border: 2px solid #000;
  background-color: #fff;
  cursor: pointer;
  transition: 0.2s ease-in;
}
.creations__btn:hover {
  background-color: #000;
  color: #fff;
}
</style>
