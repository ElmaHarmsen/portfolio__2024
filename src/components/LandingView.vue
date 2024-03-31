<script setup>
import ClickMeBtn from './ClickMeBtn.vue'
import MainHeader from './MainHeader.vue'
</script>

<template>
  <main class="landing-view-container">
    <MainHeader />
    <ClickMeBtn />
  </main>
</template>

<style scoped lang="scss">
.landing-view-container {
  display: flex;
  flex-flow: column nowrap;
  justify-content: space-between;
  padding: 2.5rem 5rem;
  min-height: 100dvh;
}
</style>
