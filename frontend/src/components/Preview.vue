<template>
  <div class="wine">
    <img :src="imageSource" :alt="imageAltText">
    <span v-if="displayBadge" class="new-badge">New!</span>
    <div v-if="progress" class="amount-consumed">
      <progress min="0" max="100" :value="progress"></progress>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Preview',
  props: {
    imageSource: String,
    imageAltText: String,
    displayBadge: Boolean,
    progress: Number,
  },
};
</script>

<style lang="scss">
</style>
