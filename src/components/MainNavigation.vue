<script setup>
import { RouterLink } from 'vue-router'
import { ref } from 'vue'

const isNavOpen = ref(false)

function openNav() {
  isNavOpen.value = !isNavOpen.value
}
</script>

<template>
  <main class="nav-container">
    <div class="nav-container__button" @click="openNav">
      <h1>menu</h1>
    </div>
    <div class="nav-container" v-if="isNavOpen">
      <RouterLink to="/" class="nav-container__item" @click="openNav">
        <h1>home page</h1>
      </RouterLink>
      <RouterLink to="/about" class="nav-container__item" @click="openNav">
        <h1>about me</h1>
      </RouterLink>
      <RouterLink to="/experience" class="nav-container__item" @click="openNav">
        <h1>experience</h1>
      </RouterLink>
      <RouterLink to="/contact" class="nav-container__item" @click="openNav">
        <h1>contact</h1>
      </RouterLink>
    </div>
  </main>
</template>

<style scoped lang="scss">
.nav-container {
  display: flex;
  flex-flow: column;
  row-gap: 1.5rem;
  align-items: end;

  &__button {
    cursor: pointer;
  }
}
</style>
