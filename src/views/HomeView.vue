<script setup>
import TitleParagraph from '../components/TitleParagraph.vue'
import CircledSection from '../components/CircledSection.vue'
import ValueSection from '../components/ValueSection.vue'
import CompetenceSection from '../components/CompetenceSection.vue'
</script>

<template>
  <main class="home-view-container">
    <TitleParagraph
      title="What's this about?"
      paragraph="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur purus quam, hendrerit at dui a, mollis fermentum mi. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Ut volutpat ultricies tortor posuere lobortis. Donec gravida tristique libero, pretium convallis mi ullamcorper et. Praesent sed ultrices felis. Donec eget purus eu nunc suscipit rutrum eget at urna. Interdum et malesuada fames ac ante ipsum primis in faucibus. Suspendisse et lorem nec lectus vulputate convallis at id augue. Donec auctor iaculis ligula, ut sagittis ipsum volutpat nec."
    />
    <CircledSection />
    <ValueSection />
    <CompetenceSection />
  </main>
</template>

<style scoped lang="scss">
.home-view-container {
  display: flex;
  flex-flow: column nowrap;
  justify-content: center;
  row-gap: var(--section-gap);
}
</style>
