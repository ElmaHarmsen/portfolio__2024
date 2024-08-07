<script setup>
import MainNavigation from '../components/MainNavigation.vue'
import HelloWorld from '../components/HelloWorld.vue'
import ExperienceSection from '../components/ExperienceSection.vue'
import AboutSection from '../components/AboutSection.vue'
import ContactSection from '../components/ContactSection.vue'
</script>

<template>
  <main>
    <MainNavigation
      homeNavItemOne="Recent Work"
      homeNavItemTwo="About Me"
      homeNavItemThree="Contact"
    />
    <HelloWorld />
    <ExperienceSection />
    <AboutSection />
    <ContactSection />
  </main>
</template>

<style lang="scss" scoped></style>
