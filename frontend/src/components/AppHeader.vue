<template>
  <header class="hero">
    <img class="hero-image" src="/wine-hero.webp">
    <nav class="navigation">
      <section class="primary-navigation">
        <h1>WineFlix</h1>
        <ul class="navigation-links">
          <li class="active">
            <a href="#">Home</a>
          </li>
          <li>
            <a href="#">Whites</a>
          </li>
          <li><a href="#">Reds</a>
          </li>
          <li><a href="#">Blends</a></li>
        </ul>
      </section>
      <section class="secondary-navigation">
        <span class="user-avatar">
          <a href="#">S</a>
        </span>
      </section>
    </nav>
    <div class="hero-content">
      <h2>
        <img alt="Rex Goliath" src="/rex-goliath-logo.png">
      </h2>
      <h3>His Royal Majesty is back.</h3>
      <p>
        America's most unhinged rooster is out of retirement, and this time? He's mad
        as hell.  Experience the unapologetic flavor burst of Rex Goliath.
      </p>
      <ul class="controls">
        <li>
          <button class="primary-action">
            <FontAwesomeIcon icon="play" />
            <span>Drink</span>
          </button>
        </li>
        <li>
          <button class="secondary-action">
            <FontAwesomeIcon icon="info-circle" />
            <span>More Info</span>
          </button>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';

export default {
  name: 'AppHeader',
  components: {
    FontAwesomeIcon,
  },
};
</script>

<style lang="scss">
</style>
