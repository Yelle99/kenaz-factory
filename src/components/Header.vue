<template>
  <header>
    <div class="primary__nav">
      <div class="container-top">
        <nav class="primary">
          <img class="logo" src="../assets/logo.svg" alt="" />
          <h1>Kenaz</h1>
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
          <ul class="nav-links">
            <li><a class="nav-news" href="#">News</a></li>
            <li><a class="nav-business" href="#">Business</a></li>
            <li><a class="nav-sport" href="#">Sport</a></li>
            <li><a class="nav-life" href="#">Life</a></li>
            <li><a class="nav-tech" href="#">Tech</a></li>
            <li><a class="nav-travel" href="#">Travel</a></li>
          </ul>
        </nav>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>
