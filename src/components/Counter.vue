<script setup>
import { ref } from "vue";
const props = defineProps({
  initialCount: Number,
});
const counter = ref(props.initialCount ?? 0);
</script>
<template>
  <slot name="top"></slot>
  <button @click="counter++">{{ counter }}</button>
  <slot name="bottom"></slot>
</template>
