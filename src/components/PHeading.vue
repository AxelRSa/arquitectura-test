<template>
  <h5 v-if="type === 'h5'">
    <slot />
  </h5>
  <h4 v-else-if="type === 'h4'">
    <slot />
  </h4>
  <h3 v-else-if="type === 'h3'">
    <slot />
  </h3>
  <h2 v-else-if="type === 'h2'">
    <slot />
  </h2>
  <h1 v-else>
    <slot />
  </h1>
</template>
<script>
export default {
  props: ['type']
}
</script>
<style scoped>
h1,
h2,
h3,
h4,
h5 {
  font-family: sans-serif;
}
</style>
