<script setup>
import { RouterView } from 'vue-router'
import LandingView from './components/LandingView.vue'
import FooterSection from './components/FooterSection.vue'
</script>

<template>
  <main class="page-container">
    <header>
      <LandingView />
    </header>
    <RouterView />
    <footer>
      <FooterSection />
    </footer>
  </main>
</template>

<style scoped lang="scss">
.page-container {
  display: flex;
  flex-flow: column nowrap;
  row-gap: var(--section-gap);
}
</style>
