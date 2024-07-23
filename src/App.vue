<script setup>
import { RouterView } from 'vue-router'
</script>

<template>
  <RouterView />
</template>

<style lang="scss">
@import './assets/reset.css';
@import './assets/fonts.css';

h1 {
  font-size: 72px;
  text-transform: uppercase;
  font-family: 'SourceSerifRegular';
}

h2 {
  font-size: 24px;
  font-family: 'SourceSerifExtraBold';
}
p {
  font-size: 16px;
  line-height: 1.5;
  font-family: 'SourceSerifSemiBold';
}
</style>
