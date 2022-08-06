<template>
  <div>
    <footer>
      <div class="container-lg">
        <div class="row align-item-start justify-content-between">
          <div class="col-lg-2 col-sm-3 col-6">
            <h4>Product</h4>
            <a href="">Follow To Earn</a>
            <a href="">Comment To Earn</a>
            <a href="">Like To Earn</a>
          </div>
          <div class="col-lg-2 col-sm-3 col-6">
            <h4>Resources</h4>
            <a href="">What is DripAda</a>
            <a href="">How it works</a>
            <a href="">DOCS</a>
          </div>
          <div class="col-lg-2 col-sm-3 col-12">
            <h4>Company</h4>
            <a href="">About Us</a>
            <a href="">Career</a>
            <a href="">Press</a>
          </div>
          <div class="col-lg-4 col-sm-8 col-12">
            <h4 class="newsletter">Newsletter</h4>
            <div class="row-item">
              <input type="text" placeholder="Enter your Email" />
              <button>Subscribe</button>
            </div>

            <div class="social-media">
              <a href=""><img src="@/assets/icons/twitter.svg" alt="" /></a>
              <a href=""><img src="@/assets/icons/instagram.svg" alt="" /></a>
              <a href=""><img src="@/assets/icons/linkedIn.svg" alt="" /></a>
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
</script>

<style>
</style>