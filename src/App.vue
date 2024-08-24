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
  font-size: 52px;
  line-height: 1.2;
  font-family: 'NotoSans-ExtraBold';
  text-transform: uppercase;
  font-variant: small-caps;
}

h2 {
  font-size: 16px;
  font-family: 'NotoSans-Bold';
  text-transform: uppercase;
  font-variant: small-caps;
}

h3 {
  font-size: 16px;
  font-family: 'NotoSans-Bold';
}

p {
  font-size: 16px;
  line-height: 1.5;
  font-family: 'NotoSans-SemiBold';
  text-align: justify;
}

@media (min-width: 1024px) {
  h1 {
    font-size: 82px;
  }

  h2 {
    font-size: 20px;
  }

  h3 {
    font-size: 20px;
  }

  p {
    font-size: 20px;
  }
}
</style>
