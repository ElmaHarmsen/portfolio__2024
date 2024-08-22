<script setup>
const scrollIntoView = (id) => {
  if (!id) return
  const elementInQuestion = document.getElementById(id)
  if (!elementInQuestion) return
  elementInQuestion.scrollIntoView({ behavior: 'smooth' })
}
</script>

<template>
  <section class="main-navigation">
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

<style lang="scss" scoped>
.nav-line {
  display: block;
  width: 100%;
  height: 0.5rem;
  background-color: black;
}

.main-navigation {
  position: absolute;
  top: 2.5rem;
  left: 50%;
  transform: translateX(-50%);
  width: calc(100% - (2 * 10%));
  display: grid;
  grid-template-columns: auto 1fr auto 1fr auto;
  grid-template-rows: 1fr;
  gap: 1rem;
  align-items: center;
  padding: 0 2.5rem;

  .content-item {
    h2 {
      cursor: pointer;
    }
  }
}
</style>
