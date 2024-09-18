<script setup>
import { ref } from 'vue'
const homeNavOpen = ref(false)

const scrollIntoView = (id) => {
  if (!id) return
  const elementInQuestion = document.getElementById(id)
  if (!elementInQuestion) return
  elementInQuestion.scrollIntoView({ behavior: 'smooth' })
}
</script>

<template>
  <section>
    <div class="navigation-btn" @click="homeNavOpen = !homeNavOpen">
      <span class="navigation-btn__line"></span>
      <span class="navigation-btn__line"></span>
      <span class="navigation-btn__line"></span>
    </div>
    <div class="navigation-small-nav" v-if="homeNavOpen">
      <router-link to="/experience" class="flex-container">
        <h2>All works</h2>
        <img class="arrow-img" src="../assets/imgs/arrow-forward.svg" alt="" />
      </router-link>
      <div class="flex-container-col">
        <h2 @click="scrollIntoView('experience-section', (homeNavOpen = false))">Selected Works</h2>
        <h2 @click="scrollIntoView('about-section', (homeNavOpen = false))">About Me</h2>
        <a
          href="https://drive.google.com/file/d/1J9CPMHknzn4jkXvPhInI-_E-kEYkzQ51/view?usp=sharing"
          target="_blank"
          @click="homeNavOpen = false"
        >
          <h2>Curriculum Vitae</h2>
        </a>
      </div>
    </div>
    <div class="navigation-container">
      <div class="content-item">
        <h2 @click="scrollIntoView('experience-section')">Selected Works</h2>
      </div>
      <span class="nav-line"></span>
      <div class="content-item">
        <h2 @click="scrollIntoView('about-section')">About Me</h2>
      </div>
      <span class="nav-line"></span>
      <div class="content-item">
        <a
          href="https://drive.google.com/file/d/1J9CPMHknzn4jkXvPhInI-_E-kEYkzQ51/view?usp=sharing"
          target="_blank"
        >
          <h2>Curriculum Vitae</h2>
        </a>
      </div>
    </div>
  </section>
</template>
