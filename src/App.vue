<script setup>
const color = '255 0 0'
</script>

<template>
  <div class="headline">Headline</div>
</template>

<style lang="scss">
.headline {
  // works:
  // --color: v-bind(color);
  // color: rgb(var(--color));

  // doesn't work
  color: rgb(v-bind(color));
}
</style>
