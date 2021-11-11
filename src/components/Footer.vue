<template>
  <footer id="footer">
    <div class="center">
      <h4 class="footer__title">loopstudios</h4>
      <ul class="footer__about">
        <li><a href="#">About</a></li>
        <li><a href="#">Careers</a></li>
        <li><a href="#">Events</a></li>
        <li><a href="#">Products</a></li>
        <li><a href="#">Support</a></li>
      </ul>
      <div class="footer__social">
        <img src="../assets/icon-facebook.svg" alt="icon-facebook" />
        <img src="../assets/icon-twitter.svg" alt="icon-twitter" />
        <img src="../assets/icon-pinterest.svg" alt="icon-pinterest" />
        <img src="../assets/icon-instagram.svg" alt="icon-instagram" />
      </div>
      <span class="footer__copyright"
        >© 2021 Loopstudios. All rights reserved.</span
      >
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style>
#footer {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  background-color: #000;
  color: #fff;
  margin-top: 120px;
  padding: 20px 0 30px;
}
#footer .center {
  row-gap: 30px;
}
.footer__title {
  font-size: 2.54em;
}
.footer__about {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  row-gap: 35px;
}
.footer__about li {
  list-style: none;
}
.footer__about a {
  font-size: 1.25em;
  letter-spacing: 1px;
  font-weight: 300;
  color: #fff;
  text-decoration: none;
}
.footer__social {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 24px;
}
.footer__social img {
  position: relative;
  height: 35px;
  width: 35px;
}
.footer__social img:hover {
  cursor: pointer;
}
.footer__copyright {
  font-size: 1.3em;
  color: var(--Dark-Gray);
  padding: 0 40px;
  text-align: center;
}
</style>
