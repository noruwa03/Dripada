<template>
  <div>
    <footer>
      <div class="container-lg">
        <div class="row align-item-start justify-content-between">
          <div class="col-lg-2 col-sm-3 col-6">
            <h4>Product</h4>
            <a class="footer-link" href="">Follow To Earn</a>
            <a class="footer-link" href="">Comment To Earn</a>
            <a class="footer-link" href="">Like To Earn</a>
          </div>
          <div class="col-lg-2 col-sm-3 col-6">
            <h4>Resources</h4>
            <a class="footer-link" href="">What is DripAda</a>
            <a class="footer-link" href="">How it works</a>
            <a class="footer-link" href="">DOCS</a>
          </div>
          <div class="col-lg-2 col-sm-3 col-12">
            <h4>Company</h4>
            <a class="footer-link" @click="aboutUs">About Us</a>
            <a class="footer-link" href="">Career</a>
            <a class="footer-link" href="">Press</a>
          </div>
          <div class="col-lg-4 col-sm-8 col-12">
            <h4 class="newsletter">Newsletter</h4>
            <div class="row-item">
              <input type="text" placeholder="Enter your Email" />
              <button>Subscribe</button>
            </div>

            <div class="social-media">
              <a href=""><img src="@/assets/icons/twitter.svg" alt="" /></a>
              <a href=""><img src="@/assets/icons/telegram.svg" alt="" /></a>
              <a href=""><img src="@/assets/icons/email.svg" alt="" /></a>
            </div>
          </div>
        </div>

        <div class="text-center footer-logo">
          <img src="@/assets/icons/footer-logo.svg" alt="" />
        </div>
        <p class="text-center">&copy; {{ footerDate }} All Rights Reserved</p>
      </div>
    </footer>
  </div>
</template>

<script setup>
const footerDate = new Date().getFullYear();
const aboutUs = () => {
  const elToView = document.getElementById("about-us");
  elToView.scrollIntoView();
};
</script>

<style>
</style>