<script setup>
import TitleParagraph from '@/components/TitleParagraph.vue'
import ImageCarousel from '@/components/ImageCarousel.vue'
</script>

<template>
  <main class="experience-view-container">
    <TitleParagraph
      title="some title here"
      paragraph="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur purus quam, hendrerit at dui a, mollis fermentum mi. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Ut volutpat ultricies tortor posuere lobortis. Donec gravida tristique libero, pretium convallis mi ullamcorper et. Praesent sed ultrices felis. Donec eget purus eu nunc suscipit rutrum eget at urna. Interdum et malesuada fames ac ante ipsum primis in faucibus. Suspendisse et lorem nec lectus vulputate convallis at id augue. Donec auctor iaculis ligula, ut sagittis ipsum volutpat nec."
    />
    <TitleParagraph title="education" />
    <ImageCarousel />
  </main>
</template>

<style scoped lang="scss">
.experience-view-container {
  display: flex;
  flex-flow: column nowrap;
  justify-content: center;
  row-gap: var(--section-gap);
}
</style>
