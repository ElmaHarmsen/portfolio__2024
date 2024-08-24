<script setup>
const scrollIntoView = (id) => {
  if (!id) return
  const elementInQuestion = document.getElementById(id)
  if (!elementInQuestion) return
  elementInQuestion.scrollIntoView({ behavior: 'smooth' })
}
</script>

<template>
  <section>
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
