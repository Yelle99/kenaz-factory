<template>
  <footer>
    <div class="footer-container">
      <div class="top-footer">
        <div class="info-row">
          <div class="kenaz-column">
            <div class="logo">
              <img src="../assets/logo-blue.svg" alt="" />
              <h1>Kenaz</h1>
            </div>
            <p class="text">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Provident, fugit vel!
            </p>
            <div class="icons">
              <div class="wifi icon"></div>
              <div class="facebook icon">
                <img src="../assets/icon2.svg" alt="" />
              </div>
              <div class="twitter icon">
                <img src="../assets/icon3.svg" alt="" />
              </div>
              <div class="ball icon"></div>
              <div class="empty icon"></div>
              <div class="youtube icon"></div>
              <div class="skype icon"></div>
            </div>
          </div>
          <div class="newsletter-column">
            <h1 class="heading">Newsletter</h1>
            <p class="text">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Provident, fugit vel!
            </p>
            <form class="subscribe">
              <input
                class="subscribe-input"
                placeholder="Your mail"
                type="text"
              />
              <button class="subscribe-btn">Subscribe</button>
            </form>
          </div>
          <div class="tags-column">
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
          </div>
        </div>
        <div class="news-row">
          <div class="featured-column">
            <FooterNews footerHeading="Featured" newsType="featured" />
          </div>
          <div class="random-column">
            <FooterNews footerHeading="Random Posts" newsType="randomposts" />
          </div>
          <div class="twitter-column">
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
