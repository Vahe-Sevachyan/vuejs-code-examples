<script setup>
import InterpolationDataBinding from "./components/InterpolationDataBinding.vue";
import Events from "./components/Events.vue";
</script>

<template>
  <InterpolationDataBinding />
  <Events />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
