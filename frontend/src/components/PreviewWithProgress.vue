<template>
  <div class="wine">
    <img :src="imageSource" :alt="imageAltText">
    <span v-if="displayBadge" class="new-badge">New!</span>
  </div>
</template>

<script>
export default {
  name: 'Preview',
  props: {
    imageSource: String,
    imageAltText: String,
    displayBadge: Boolean,
  },
};
</script>

<style lang="scss">
</style>
