<script setup>
import { ref, computed } from "vue";
import { useMouse } from "@vueuse/core";
const { x, y } = useMouse();

const el = ref();
const cssRotate = computed(() => {
  if (!el.value) return;
  const rect = el.value.getBoundingClientRect();
  const centerX = rect.left + rect.width / 2;
  const centerY = rect.top + rect.height / 2;

  const deltaX = x.value - centerX;
  const deltaY = y.value - centerY;

  const rad = Math.atan2(deltaY, deltaX);
  const deg = rad * (180 / Math.PI) + 90; // +90 to offset the default rotation

  return `rotate(${deg}deg)`;
});
</script>
<template>
  <span ref="el" id="rotateMe">👩‍🚀</span>
</template>
<style scoped>
#rotateMe {
  transform-origin: center center;
  transform: v-bind(cssRotate);
  display: inline-block;
}
</style>
