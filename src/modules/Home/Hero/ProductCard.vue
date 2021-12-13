<template>
  <div class="hola">
    <PText>{{ description }}</PText>
  </div>
</template>
<script>
import PText from '@/components/PText.vue'
export default {
  components: {
    PText
  },
  props: ['description']
}
</script>
<style scoped>
div {
  background-color: blue;
}
</style>
