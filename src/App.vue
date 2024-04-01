<script setup>
import { RouterView } from 'vue-router'
import { onMounted } from 'vue'
import { register } from 'swiper/element/bundle'
import LandingView from './components/LandingView.vue'
import FooterSection from './components/FooterSection.vue'

onMounted(() => {
  register()
})
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
