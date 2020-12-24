<template>
  <header class="hero">
    <img class="hero-image" src="/wine-hero.webp">
    <NavBar :navLinks="navLinks" :avatarInitial="avatarInitial" />
    <HeroContent
      :imageAltText="hero.imageAltText"
      :imageSource="hero.imageSource"
      :head="hero.head"
      :description="hero.description"
    />
  </header>
  <main>
    <section class="category">
      <h2>Drink Again</h2>
      <ul>
        <li v-for="preview in drinkAgain" :key="preview.id">
          <Preview :imageSource="preview.imageSource"
                   :imageAltText="preview.imageAltText"
                   :displayBadge="preview.displayBadge"
                   :progress="preview.progress"
          />
        </li>
      </ul>
    </section>
    <section class="category">
      <h2>Keep Drinking</h2>
      <ul>
        <li v-for="preview in keepDrinking" :key="preview.id">
          <Preview :imageSource="preview.imageSource"
                   :imageAltText="preview.imageAltText"
                   :displayBadge="preview.displayBadge"
                   :progress="preview.progress"
          />
        </li>
      </ul>
    </section>
  </main>
</template>

<script>
import NavBar from '@/components/NavBar.vue';
import HeroContent from '@/components/HeroContent.vue';
import Preview from '@/components/Preview.vue';

export default {
  name: 'App',
  components: {
    NavBar,
    HeroContent,
    Preview,
  },
  data() {
    return {
      navLinks: [
        {
          name: 'Home',
          link: '#',
        },
        {
          name: 'Whites',
          link: '#',
        },
        {
          name: 'Reds',
          link: '#',
        },
        {
          name: 'Blends',
          link: '#',
        },
      ],
      hero: {
        imageAltText: 'Rex Goliath',
        imageSource: '/rex-goliath-logo.png',
        head: 'His Royal Majesty is back.',
        description: "America's most unhinged rooster is out of retirement, and this time? He's mad as hell.  Experience the unapologetic flavor burst of Rex Goliath.",
      },
      drinkAgain: [
        {
          id: 1,
          imageAltText: 'Wine',
          imageSource: '/red-wine.jpg',
          displayBadge: true,
        },
        {
          id: 2,
          imageAltText: 'Wine',
          imageSource: '/red-wine.jpg',
          displayBadge: true,
        },
        {
          id: 3,
          imageAltText: 'Wine',
          imageSource: '/red-wine.jpg',
          displayBadge: false,
        },
        {
          id: 4,
          imageAltText: 'Wine',
          imageSource: '/red-wine.jpg',
          displayBadge: true,
        },
        {
          id: 5,
          imageAltText: 'Wine',
          imageSource: '/red-wine.jpg',
          displayBadge: false,
        },
        {
          id: 6,
          imageAltText: 'Wine',
          imageSource: '/red-wine.jpg',
          displayBadge: false,
        },
        {
          id: 7,
          imageAltText: 'Wine',
          imageSource: '/red-wine.jpg',
          displayBadge: false,
        },
        {
          id: 8,
          imageAltText: 'Wine',
          imageSource: '/red-wine.jpg',
          displayBadge: false,
        },
      ],
      keepDrinking: [
        {
          id: 1,
          imageAltText: 'Wine',
          imageSource: '/red-wine.jpg',
          displayBadge: false,
          progress: 22,
        },
        {
          id: 2,
          imageAltText: 'Wine',
          imageSource: '/red-wine.jpg',
          displayBadge: false,
          progress: 22,
        },
        {
          id: 3,
          imageAltText: 'Wine',
          imageSource: '/red-wine.jpg',
          displayBadge: false,
          progress: 22,
        },
        {
          id: 4,
          imageAltText: 'Wine',
          imageSource: '/red-wine.jpg',
          displayBadge: false,
          progress: 22,
        },
        {
          id: 5,
          imageAltText: 'Wine',
          imageSource: '/red-wine.jpg',
          displayBadge: false,
          progress: 22,
        },
        {
          id: 6,
          imageAltText: 'Wine',
          imageSource: '/red-wine.jpg',
          displayBadge: false,
          progress: 22,
        },
        {
          id: 7,
          imageAltText: 'Wine',
          imageSource: '/red-wine.jpg',
          displayBadge: false,
          progress: 22,
        },
        {
          id: 8,
          imageAltText: 'Wine',
          imageSource: '/red-wine.jpg',
          displayBadge: false,
          progress: 22,
        },
      ],
    };
  },
  computed: {
    avatarInitial() {
      return 'J';
    },
  },
};
</script>

<style lang="scss">
</style>
