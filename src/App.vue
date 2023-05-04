<script>
import HeaderComp from './components/HeaderComp.vue'

export default {
  name: "app",
  components: {
    HeaderComp
  }
}
</script>

<template>
  <!-- NAVBAR -->
  <HeaderComp />

  <!-- CONTENT -->
  <div class="content">
    <h1><a href="#">Content gose here</a></h1>
  </div>

  <!-- MERCHANDISE -->
  <section class="bg-blue">

    <div class="merch">

      <img src="/img/buy-comics-digital-comics.png" alt="immagine digital comics">
      <span class="white">DIGITAL COMICS</span>

    </div>

    <div class="merch">

      <img src="/img/buy-comics-merchandise.png" alt="immagine merchandise comics">
      <span class="white">DC MERCHANDISE</span>

    </div>

    <div class="merch">

      <img src="/img/buy-comics-subscriptions.png" alt="immagine subscrption comics">
      <span class="white">SUBSCRIPTION</span>

    </div>

    <div class="merch">

      <img src="/img/buy-comics-shop-locator.png" alt="immagine shop location">
      <span class="white">COMICS SHOP LOCATION</span>

    </div>

    <div class="merch">

      <img class="carta" src="/img/buy-dc-power-visa.svg" alt="immagine carta di credito">
      <span class="white">DC POWER VISA</span>

    </div>

  </section>

  <!-- LISTE DI LINK -->
  <section id="riassunto">

    <div id="last">

      <div id="liste">

        <div>

          <ul>
            <span class="titolo-lista white">DC COMICS</span>
            <li>
              <a href="#">Characters</a>
            </li>
            <li>
              <a href="#">Comics</a>
            </li>
            <li>
              <a href="#">Movies</a>
            </li>
            <li>
              <a href="#">TV</a>
            </li>
            <li>
              <a href="#">Games</a>
            </li>
            <li>
              <a href="#">Videos</a>
            </li>
            <li>
              <a href="#">News</a>
            </li>
          </ul>

          <ul>
            <span class="titolo-lista white">SHOP</span>
            <li>
              <a href="#">Shop DC</a>
            </li>
            <li>
              <a href="#">Shop DC Collectibles</a>
            </li>
          </ul>

        </div>

        <ul>
          <span class="titolo-lista white">DC</span>
          <li>
            <a href="#">Terms Of Use</a>
          </li>
          <li>
            <a href="#">Privacy policy (New)</a>
          </li>
          <li>
            <a href="#">Ad Choices</a>
          </li>
          <li>
            <a href="#">Advertising</a>
          </li>
          <li>
            <a href="#">Jobs</a>
          </li>
          <li>
            <a href="#">Subscription</a>
          </li>
          <li>
            <a href="#">Talent Workshops</a>
          </li>
          <li>
            <a href="#">CPSC Certificates</a>
          </li>
          <li>
            <a href="#">Ratings</a>
          </li>
          <li>
            <a href="#">Shop Help</a>
          </li>
          <li>
            <a href="#">Contact Us</a>
          </li>
        </ul>

        <ul>
          <span class="titolo-lista white">SITES</span>
          <li>
            <a href="#">DC</a>
          </li>
          <li>
            <a href="#">MAD Magazine</a>
          </li>
          <li>
            <a href="#">DC Kids</a>
          </li>
          <li>
            <a href="#">DC Universe</a>
          </li>
          <li>
            <a href="#">DC Pover Visa</a>
          </li>
        </ul>


      </div>

      <div id="logo">
        <img src="/img/dc-logo-bg.png" alt="">
      </div>

    </div>

  </section>

  <!-- ISCRIZIONE E SOCIAL -->
  <footer>

    <div id="finale">

      <button>
        <span class="white">SIGN-UP NOW!</span>
      </button>

      <div>
        <span id="follow">FOLLOW US</span>
        <img src="/img/footer-facebook.png" alt="social facebook">
        <img src="/img/footer-twitter.png" alt="social twitter">
        <img src="/img/footer-youtube.png" alt="youtube logo">
        <img src="/img/footer-pinterest.png" alt="social pinterest">
        <img src="/img/footer-periscope.png" alt="periscope logo">
      </div>

    </div>
  </footer>
</template>

<style lang="scss">
@use './style/main.scss' as *;
</style>
