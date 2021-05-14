<template>
  <footer>
    <div class="container">
      <div class="top-footer">
        <div class="first-row">
          <div class="logo">
            <img src="../assets/logo-blue.svg" alt="" />
            <h1>Kenaz</h1>
          </div>
          <p class="text">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Provident,
            fugit vel!
          </p>
          <div class="icons">
            <div class="wifi"></div>
            <div class="facebook">
              <img src="../assets/icon2.svg" alt="" />
            </div>
            <div class="twitter">
              <img src="../assets/icon3.svg" alt="" />
            </div>
            <div class="ball"></div>
            <div class="empty"></div>
            <div class="youtube"></div>
            <div class="skype"></div>
          </div>
          <FooterNews footerHeading="Featured" newsType="featured" />
        </div>
        <div class="second-row">
          <h1 class="heading">Newsletter</h1>
          <p class="text">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Provident,
            fugit vel!
          </p>
          <form class="subscribe">
            <input
              class="subscribe-input"
              placeholder="Your mail"
              type="text"
            />
            <button class="subscribe-btn">Subscribe</button>
          </form>
          <FooterNews footerHeading="Random Posts" newsType="randomposts" />
        </div>
        <div class="third-row">
          <h1 class="heading">Tags Widget</h1>
          <div class="tags">
            <span>assueverit</span>
            <span>utroquoe</span>
            <span>probo</span>
            <span>assuev</span>
            <span>probo</span>
            <span>asuevverit</span>
            <span>titl</span>
            <span class="active">asuevverit</span>
            <span>asuevverit</span>
            <span>utroquoe</span>
            <span>probo</span>
            <span>asuevverit</span>
            <span>utroquoe</span>
          </div>
          <h1 class="twitter-feed">Twitter Feed</h1>
          <div class="twitter-post">
            <img src="../assets/twitter-bird.svg" alt="" />
            <span class="twitter-username">Envato @envato</span>
            <p class="twitter-text">
              Is this your typical million dollar day in the park?
              http://enva.to/150vxFC Happy @TrueThemes Day! #ThemeForest
              pic.twitter.com/EHz7awxOXy
            </p>
          </div>
          <div class="twitter-post">
            <img src="../assets/twitter-bird.svg" alt="" />
            <span class="twitter-username">Envato @envato</span>
            <p class="twitter-text">
              Happy TrueThemes Day http://enva.to/1dRzgLD
            </p>
          </div>
          <div class="twitter-post">
            <img src="../assets/twitter-bird.svg" alt="" />
            <span class="twitter-username">Envato @envato</span>
            <p class="twitter-text">
              @robscri I would really want to look into what's taking so long.
              Thank you ever so much! ^TC
            </p>
          </div>
        </div>
      </div>
      <div class="bottom-footer">
        <span
          >&copy; 2013 - Kenaz Template - Proudly made at Plava tvornica Croatia
        </span>
        <span>
          <a href="#">Typography</a> - <a href="#">Templates</a> -
          <a href="#">Contact Form</a> -
          <a href="#">404 page</a>
        </span>
      </div>
    </div>
  </footer>
</template>

<script>
import FooterNews from "./FooterNews";

export default {
  name: "Footer",
  components: {
    FooterNews,
  },
};
</script>
