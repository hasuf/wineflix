<template>
  <span class='user-avatar'>
    <a href="#">{{initials}}</a>
  </span>
</template>

<script>
export default {
  name: 'Avatar',
  props: {
    initials: String,
  },
};
</script>

<style lang="scss">
</style>
