<template>
  <nav class="navigation">
    <section class="primary-navigation">
      <h1>WineFlix</h1>
      <ul class="navigation-links">
        <li v-for="link in navLinks" :key="link.name" >
          <NavLink :link="link.link" :name="link.name" />
        </li>
      </ul>
    </section>
    <section class="secondary-navigation">
      <Avatar :initials='avatarInitial'/>
    </section>
  </nav>
</template>

<script>
import Avatar from '@/components/Avatar.vue';
import NavLink from '@/components/NavLink.vue';

export default {
  name: 'NavBar',
  components: {
    Avatar,
    NavLink,
  },
  props: {
    navLinks: Array,
    avatarInitial: String,
  },
};
</script>

<style lang="scss">
</style>
