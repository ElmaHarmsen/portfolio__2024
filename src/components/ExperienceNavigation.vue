<script setup>
import { ref } from 'vue'
const experienceNavOpen = ref(false)

const scrollIntoView = (id) => {
  if (!id) return
  const elementInQuestion = document.getElementById(id)
  if (!elementInQuestion) return
  elementInQuestion.scrollIntoView({ behavior: 'smooth' })
}
</script>

<template>
  <section>
    <div class="navigation-btn" @click="experienceNavOpen = !experienceNavOpen">
      <span class="navigation-btn__line"></span>
      <span class="navigation-btn__line"></span>
      <span class="navigation-btn__line"></span>
    </div>
    <div class="navigation-small-nav" v-if="experienceNavOpen">
      <router-link to="/" class="flex-container">
        <img class="arrow-img" src="../assets/imgs/arrow-back.svg" alt="" />
        <h2>Home</h2>
      </router-link>
      <div class="flex-container-col">
        <h2 @click="scrollIntoView('ux-project-section', (experienceNavOpen = false))">
          The UX Case
        </h2>
        <h2 @click="scrollIntoView('daily-ui-section', (experienceNavOpen = false))">Daily UI's</h2>
        <h2 @click="scrollIntoView('research-section', (experienceNavOpen = false))">
          Robot & AI Research
        </h2>
      </div>
    </div>
    <div class="navigation-container">
      <div class="content-item">
        <h2 @click="scrollIntoView('ux-project-section')">The UX Case</h2>
        <div class="content-item__nav-active"></div>
      </div>
      <span class="nav-line"></span>
      <div class="content-item">
        <h2 @click="scrollIntoView('daily-ui-section')">Daily UI's</h2>
        <div class="content-item__nav-active"></div>
      </div>
      <span class="nav-line"></span>
      <div class="content-item">
        <h2 @click="scrollIntoView('research-section')">Robot & AI Research</h2>
        <div class="content-item__nav-active"></div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.flex-container {
  transform: translateX(-0.25rem);
}
</style>
