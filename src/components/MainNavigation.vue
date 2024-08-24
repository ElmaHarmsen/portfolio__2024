<script setup>
const scrollIntoView = (id) => {
  if (!id) return
  const elementInQuestion = document.getElementById(id)
  if (!elementInQuestion) return
  elementInQuestion.scrollIntoView({ behavior: 'smooth' })
}
</script>

<template>
  <section class="navigation-container">
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
        href="https://drive.google.com/file/d/1UZjNtQ9nmxyYSvrw8UkutdDfxknvxHN2/view?usp=sharing"
        target="_blank"
      >
        <h2>Curriculum Vitae</h2>
      </a>
    </div>
  </section>
</template>
