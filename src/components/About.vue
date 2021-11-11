<template>
  <article id="about">
    <img
      class="about__img"
      src="../assets/mobile/image-interactive.jpg"
      alt=""
    />
    <div class="about__container">
      <h3 class="subtitle">The leader in interactive VR</h3>
      <p class="about__info">
        Founded in 2011, loopstudios has been producing world-class virtual
        reality project for some of the best companies around the globe. Our
        award-winning creations have transformed businesses through digital
        experiences that bind to their brand.
      </p>
    </div>
  </article>
</template>

<script>
export default {};
</script>

<style>
#about {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  padding: 120px 28px 50px;
  text-align: center;
}
.about__img {
  width: 100%;
}
.about__info {
  color: var(--Dark-Gray);
  font-size: 1.125em;
  line-height: 31px;
  max-width: 318px;
}
</style>
