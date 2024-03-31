<script setup>
import MainNavigation from './MainNavigation.vue'
</script>

<template>
  <main>
    <div class="header-container">
      <h1>Elma Harmsen</h1>
      <MainNavigation />
    </div>
  </main>
</template>

<style scoped lang="scss">
.header-container {
  display: flex;
  flex-flow: row nowrap;
  justify-content: space-between;
  width: 100%;
}
</style>
