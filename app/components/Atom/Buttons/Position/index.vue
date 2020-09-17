<template>
  <button
    class="btn btn--position"
    @mouseenter.stop="mouseEvent($event)"
    @mouseleave.prevent="mouseEvent($event)"
  >
    Position<span ref="circlePosition"></span>
  </button>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'Position',
  methods: {
    mouseEvent(event: any) {
      const point: any = this.$refs.circlePosition
      point.style.top = event.offsetY + 'px'
      point.style.left = event.offsetX + 'px'
    },
  },
})
</script>
<style lang="stylus" src="./index.stylus" scoped />
