<template>
  <div>
    <footer>
      <div class="container-lg">
        <div class="row align-item-start justify-content-between">
          <div class="col-lg-2 col-sm-3 col-6">
            <h4>Product</h4>
            <NuxtLink
              class="footer-link"
              to="https://resources.dripada.com/products/follow-to-earn"
              target="_blank"
            >
              Follow To Earn
            </NuxtLink>
            <NuxtLink
              class="footer-link"
              to="https://resources.dripada.com/products/comment-to-earn"
              target="_blank"
            >
              Comment To Earn
            </NuxtLink>
            <NuxtLink
              class="footer-link"
              to="https://resources.dripada.com/products/like-to-earn"
              target="_blank"
            >
              Like To Earn
            </NuxtLink>
          </div>
          <div class="col-lg-2 col-sm-3 col-6">
            <h4>Resources</h4>
            <NuxtLink
              class="footer-link"
              to="https://resources.dripada.com"
              target="_blank"
            >
              What is DripAda
            </NuxtLink>
            <NuxtLink class="footer-link"> How it works </NuxtLink>
            <NuxtLink class="footer-link"> DOCS </NuxtLink>
          </div>
          <div class="col-lg-2 col-sm-3 col-12">
            <h4>Company</h4>
            <a class="footer-link" @click="aboutUs">About Us</a>
            <NuxtLink
              class="footer-link"
              to="https://resources.dripada.com/career"
              target="_blank"
            >
              Career
            </NuxtLink>
            <NuxtLink
              class="footer-link"
              to="https://resources.dripada.com/press"
              target="_blank"
            >
              Press
            </NuxtLink>
          </div>
          <div class="col-lg-4 col-sm-8 col-12">
            <h4 class="newsletter">Newsletter</h4>
            <div class="row-item">
              <input type="text" placeholder="Enter your Email" />
              <button>Subscribe</button>
            </div>

            <div class="social-media">
              <NuxtLink to="https://twitter.com/drip_ada" target="_blank">
                <img src="@/assets/icons/twitter.svg" alt="Twitter" />
              </NuxtLink>
              <NuxtLink to="https://t.me/dripadacommunity" target="_blank">
                <img src="@/assets/icons/telegram.svg" alt="Telegram" />
              </NuxtLink>
              <NuxtLink
                to="https://instagram.com/dripadacommunity"
                target="_blank"
              >
                <img src="@/assets/icons/instagram.svg" alt="Instagram" />
              </NuxtLink>
            </div>
          </div>
        </div>

        <div class="text-center footer-logo">
          <img src="@/assets/icons/footer-logo.svg" alt="Footer Logo" />
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