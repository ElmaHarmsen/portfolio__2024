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
          <h2>Home</h2>
          <img
            class="line-image"
            src="../assets/imgs/menu-underline-home.png"
            alt="line under navigation item home"
          />
        </router-link>
        <div v-if="homeNavOpen" class="content-item__navitems">
          <p @click="scrollIntoView('experience-section')">{{ homeNavItemOne }}</p>
          <p @click="scrollIntoView('about-section')">{{ homeNavItemTwo }}</p>
          <p @click="scrollIntoView('contact-section')">{{ homeNavItemThree }}</p>
        </div>
      </div>
      <div class="content-item">
        <router-link
          to="/experience"
          @click="caseNavOpen = !caseNavOpen"
          @mouseover="caseNavOpen = true"
        >
          <h2>Cases</h2>
          <img
            class="line-image"
            src="../assets/imgs/menu-underline-cases.png"
            alt="line under navigation item cases"
          />
        </router-link>
        <div v-if="caseNavOpen" class="content-item__navitems">
          <p @click="scrollIntoView('daily-ui-section')">{{ caseNavItemOne }}</p>
          <p @click="scrollIntoView('ux-project-section')">{{ caseNavItemTwo }}</p>
          <p @click="scrollIntoView('research-section')">{{ caseNavItemThree }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.main-navigation {
  position: absolute;
  top: 40px;
  left: 40px;

  &__button {
    cursor: pointer;
    .image {
      width: 40px;
    }
  }

  &__content-wrapper {
    display: flex;
    flex-flow: row nowrap;
    justify-content: space-between;
    column-gap: 80px;

    .content-item {
      display: flex;
      flex-flow: column nowrap;
      row-gap: 20px;

      h2 {
        text-transform: uppercase;
      }

      .line-image {
        width: 60px;
        transform: translateX(-5px) translateY(-5px);
      }

      &__navitems {
        position: absolute;
        top: 40px;
        display: flex;
        flex-flow: column nowrap;
        row-gap: 5px;

        p {
          cursor: pointer;
        }
      }
    }
  }
}
</style>
