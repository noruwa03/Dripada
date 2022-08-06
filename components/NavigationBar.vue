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
            <a class="nav-link" href="">About</a>
          </li>

          <li class="nav-item">
            <a class="nav-link"
              >Products
              <span><img src="@/assets/icons/dropdown.svg" alt="" /></span>
            </a>
            <ul class="dropdown">
              <li @click="removeNavbar"><a href="">Follow To Earn</a></li>
              <li @click="removeNavbar"><a href="">Comment To Earn</a></li>
              <li @click="removeNavbar"><a href="">Like To Earn</a></li>
            </ul>
          </li>
          <li class="nav-item">
            <NuxtLink class="nav-link"
              >Company
              <span><img src="@/assets/icons/dropdown.svg" alt="" /></span
            ></NuxtLink>
            <ul class="dropdown">
              <li @click="removeNavbar"><a href="">About Us</a></li>
              <li @click="removeNavbar"><a href="">Career</a></li>
              <li @click="removeNavbar"><a href="">Press</a></li>
            </ul>
          </li>
          <li @click="removeNavbar" class="nav-item">
            <NuxtLink class="nav-link" to="">DRP Token</NuxtLink>
          </li>
        </ul>

        <a href="" class="nav-bar-beta-signup">Beta SignUp</a>
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
</script>

<style>
</style>