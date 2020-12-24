<template>
  <a :href="link">{{ name }} </a>
</template>

<script>
export default {
  name: 'NavLink',
  components: {
  },
  computed: {
  },
  props: {
    name: String,
    link: String,
  },
};
</script>

<style lang="scss">
</style>
