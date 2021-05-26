<template>
  <header>
    <div class="primary__nav">
      <div class="container-top">
        <nav class="primary">
          <div class="logo">
            <img class="logo-img" src="../assets/logo.svg" alt="" />
            <h1>Kenaz</h1>
          </div>
          <ul class="nav-links">
            <li><a href="#">Media</a></li>
            <li><a href="#">Marketing</a></li>
            <li><a href="#">Contact</a></li>
          </ul>
          <img class="search-icon" src="../assets/search-icon.svg" alt="" />
        </nav>
      </div>
    </div>
    <div class="secondary__nav">
      <div class="container-top">
        <nav class="secondary">
          <ul class="secondary-nav-links">
            <span class="close-nav" @click="closeNav">&times;</span>
            <li @click="closeNav">
              <router-link class="nav-news" to="/">News</router-link>
            </li>
            <li @click="closeNav">
              <a class="nav-business" href="#">Business</a>
            </li>
            <li @click="closeNav"><a class="nav-sport" href="#">Sport</a></li>
            <li @click="closeNav"><a class="nav-life" href="#">Life</a></li>
            <li @click="closeNav"><a class="nav-tech" href="#">Tech</a></li>
            <li @click="closeNav"><a class="nav-travel" href="#">Travel</a></li>
          </ul>
          <div class="burger" @click="openNav">
            <div></div>
            <div></div>
            <div></div>
          </div>
        </nav>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      showNav: false,
    };
  },
  methods: {
    openNav() {
      let nav = document.querySelector(".secondary-nav-links");
      let closeNav = document.querySelector(".close-nav");
      closeNav.style.display = "block";
      nav.style.visibility = "visible";
    },
    closeNav() {
      let nav = document.querySelector(".secondary-nav-links");
      let closeNav = document.querySelector(".close-nav");
      closeNav.style.display = "none";
      nav.style.visibility = "hidden";
    },
  },
};
</script>
