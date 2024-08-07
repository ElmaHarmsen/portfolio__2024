<script setup>
import MainNavigation from '../components/MainNavigation.vue'
import HelloExperience from '../components/HelloExperience.vue'
import DailyUIShowcase from '../components/DailyUIShowcase.vue'
import UXProject from '../components/UXProject.vue'
import RobotAIResearch from '../components/RobotAIResearch.vue'
</script>

<template>
  <main>
    <MainNavigation
      caseNavItemOne="Daily UI"
      caseNavItemTwo="UX Case"
      caseNavItemThree="Research"
    />
    <HelloExperience />
    <DailyUIShowcase />
    <UXProject />
    <RobotAIResearch />
  </main>
</template>
