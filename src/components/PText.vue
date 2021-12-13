<template>
  <p :class="[size === 'small' ? 'small' : size === 'big' ? 'big' : '']">
    <slot />
  </p>
</template>
<script>
export default {
  props: ['size']
}
</script>
<style scoped>
p {
  font-size: 18px;
  font-family: monospace;
}
.small {
  font-size: 16px;
}
p.big {
  font-size: 20px;
}
</style>
