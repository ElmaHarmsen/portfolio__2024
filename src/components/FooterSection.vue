<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
  <main class="nav-container">
    <RouterLink to="/" class="nav-container__item">
      <h1>home page</h1>
    </RouterLink>
    <RouterLink to="/about" class="nav-container__item">
      <h1>about me</h1>
    </RouterLink>
    <RouterLink to="/experience" class="nav-container__item">
      <h1>experience</h1>
    </RouterLink>
    <RouterLink to="/contact" class="nav-container__item">
      <h1>contact</h1>
    </RouterLink>
  </main>
</template>

<style scoped lang="scss">
.nav-container {
  display: flex;
  flex-flow: column;
  row-gap: 1.5rem;
  padding: 2.5rem 5rem;
}
</style>
