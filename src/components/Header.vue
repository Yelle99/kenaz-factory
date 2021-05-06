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
            <li><a class="news" href="#">News</a></li>
            <li><a class="business" href="#">Business</a></li>
            <li><a class="sport" href="#">Sport</a></li>
            <li><a class="life" href="#">Life</a></li>
            <li><a class="tech" href="#">Tech</a></li>
            <li><a class="travel" href="#">Travel</a></li>
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
