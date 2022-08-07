<template>
  <div>
    <nav>
      <div class="nav-item-container">
        <!-- Logo -->

        <NuxtLink class="navbar-brand logo-image" to="/"
          ><img src="@/assets/icons/logo.svg" alt="logo"
        /></NuxtLink>
        <!-- End of Logo -->

        <ul class="nav-item-list">
          <li @click="removeNavbar" class="nav-item">
            <a class="nav-link" @click="aboutUs">About</a>
          </li>

          <li class="nav-item">
            <a class="nav-link" @click="closeDropdown"
              >Products
              <span
                ><img src="@/assets/icons/dropdown.svg" alt="Dropdown Icon"
              /></span>
            </a>
            <ul class="dropdown">
              <li @click="removeNavbar">
                <NuxtLink
                  to="https://resources.dripada.com/products/follow-to-earn"
                  target="_blank"
                >
                  Follow To Earn
                </NuxtLink>
              </li>
              <li @click="removeNavbar">
                <NuxtLink
                  to="https://resources.dripada.com/products/comment-to-earn"
                  target="_blank"
                >
                  Comment To Earn
                </NuxtLink>
              </li>
              <li @click="removeNavbar">
                <NuxtLink
                  to="https://resources.dripada.com/products/like-to-earn"
                  target="_blank"
                >
                  Like To Earn
                </NuxtLink>
              </li>
            </ul>
          </li>
          <li class="nav-item">
            <a class="nav-link" @click="closeDropdown2"
              >Company
              <span
                ><img
                  src="@/assets/icons/dropdown.svg"
                  alt="Dropdown Icon" /></span
            ></a>
            <ul class="dropdown2">
              <li @click="removeNavbar"><a @click="aboutUs">About Us</a></li>
              <li @click="removeNavbar">
                <NuxtLink
                  to="https://resources.dripada.com/career"
                  target="_blank"
                >
                  Career
                </NuxtLink>
              </li>
              <li @click="removeNavbar">
                <NuxtLink
                  to="https://resources.dripada.com/press"
                  target="_blank"
                >
                  Press
                </NuxtLink>
              </li>
            </ul>
          </li>
          <li @click="removeNavbar" class="nav-item">
            <NuxtLink
              class="nav-link"
              to="https://resources.dripada.com/tokenomics"
              >DRP Token</NuxtLink
            >
          </li>
        </ul>

        <a href="" class="nav-bar-start-earning">Start Earning</a>
        <div @click="menuHandler" class="menu">
          <span></span>
          <span></span>
          <span></span>
          <span></span>
          <span></span>
          <span></span>
        </div>
      </div>
    </nav>
  </div>
</template>

<script setup>
const menuHandler = () => {
  const navItem = document.querySelector(".nav-item-list");
  const menu = document.querySelector(".menu");

  navItem.classList.toggle("active");
  menu.classList.toggle("open");
};

const removeNavbar = () => {
  const navItem = document.querySelector(".nav-item-list");
  const menu = document.querySelector(".menu");

  navItem.classList.toggle("active");
  menu.classList.toggle("open");
};

const closeDropdown = () => {
  const dropdown = document.querySelector(".dropdown");
  dropdown.classList.toggle("active");
};

const closeDropdown2 = () => {
  const dropdown2 = document.querySelector(".dropdown2");
  dropdown2.classList.toggle("active");
};

const aboutUs = () => {
  const elToView = document.getElementById("about-us");
  elToView.scrollIntoView();
};
</script>

<style>
</style>