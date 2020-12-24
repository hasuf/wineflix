<template>
  <div class="hero-content">
    <h2>
      <img :alt="imageAltText" :src="imageSource">
    </h2>
    <h3>{{ head }}</h3>
    <p>{{ description }}</p>
    <ul class="controls">
      <li>
        <HeroPlay />
      </li>
      <li>
        <HeroInfo />
      </li>
    </ul>
  </div>
</template>

<script>
import HeroPlay from '@/components/HeroPlay.vue';
import HeroInfo from '@/components/HeroInfo.vue';

export default {
  name: 'HeroContent',
  components: {
    HeroPlay,
    HeroInfo,
  },
  props: {
    description: String,
    head: String,
    imageAltText: String,
    imageSource: String,
  },
};
</script>

<style lang="scss">
</style>
