<script setup>
import { ref } from 'vue'
const homeNavOpen = ref(false)
const caseNavOpen = ref(false)
defineProps({
  homeNavItemOne: String,
  homeNavItemTwo: String,
  homeNavItemThree: String,
  caseNavItemOne: String,
  caseNavItemTwo: String,
  caseNavItemThree: String
})

const scrollIntoView = (id) => {
  if (!id) return
  const elementInQuestion = document.getElementById(id)
  if (!elementInQuestion) return
  elementInQuestion.scrollIntoView({ behavior: 'smooth' })
}
</script>

<template>
  <section class="main-navigation">
    <div class="main-navigation__content-wrapper">
      <div class="content-item">
        <router-link to="/" @click="homeNavOpen = !homeNavOpen" @mouseover="homeNavOpen = true">
          <h3>Home</h3>
        </router-link>
        <div v-if="homeNavOpen" class="content-item__navitems">
          <h3 @click="scrollIntoView('exh3erience-section')">{{ homeNavItemOne }}</h3>
          <h3 @click="scrollIntoView('about-section')">{{ homeNavItemTwo }}</h3>
          <h3 @click="scrollIntoView('contact-section')">{{ homeNavItemThree }}</h3>
        </div>
      </div>
      <div class="content-item">
        <router-link
          to="/experience"
          @click="caseNavOpen = !caseNavOpen"
          @mouseover="caseNavOpen = true"
        >
          <h3>Cases</h3>
        </router-link>
        <div v-if="caseNavOpen" class="content-item__navitems">
          <h3 @click="scrollIntoView('daily-ui-section')">{{ caseNavItemOne }}</h3>
          <h3 @click="scrollIntoView('ux-h3roject-section')">{{ caseNavItemTwo }}</h3>
          <h3 @click="scrollIntoView('research-section')">{{ caseNavItemThree }}</h3>
        </div>
      </div>
      <div class="content-item">
        <a
          href="https://drive.google.com/file/d/1UZjNtQ9nmxyYSvrw8UkutdDfxknvxHN2/view?usp=sharing"
          target="_blank"
        >
          <h3>Curriculum Vitae</h3>
        </a>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.main-navigation {
  position: absolute;
  top: 40px;
  width: 100%;

  &__content-wrapper {
    display: flex;
    flex-flow: row nowrap;
    justify-content: center;
    column-gap: 50px;

    .content-item {
      display: flex;
      flex-flow: column nowrap;
      row-gap: 20px;

      &__navitems {
        position: absolute;
        top: 40px;
        display: flex;
        flex-flow: column nowrap;
        row-gap: 5px;

        h3 {
          cursor: pointer;
        }
      }
    }
  }
}
</style>
