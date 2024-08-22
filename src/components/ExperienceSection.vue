<script setup>
const scrollIntoView = (id) => {
  if (!id) return
  const elementInQuestion = document.getElementById(id)
  if (!elementInQuestion) return
  elementInQuestion.scrollIntoView({ behavior: 'smooth' })
}
</script>

<template>
  <section class="section-grid" id="experience-section">
    <div class="section-grid__content">
      <div class="section-navigation">
        <h2 @click="scrollIntoView('daily-ui-section')">Daily UI's</h2>
        <span class="nav-line"></span>
        <h2>The UX Case</h2>
        <span class="nav-line"></span>
        <h2>Robot & AI Research</h2>
      </div>
      <div class="content-item">
        <h1>
          Selected <br />
          Works
        </h1>
      </div>
    </div>
    <div class="circle-element"></div>
  </section>
</template>

<style lang="scss" scoped>
.circle-element {
  background: radial-gradient(ellipse at top right, #ff9a44, transparent),
    radial-gradient(circle at bottom left, #fc6076, transparent);
  opacity: 0.95;
  width: 600px;
  height: 600px;
  border-radius: 300px 300px 300px 400px;
  filter: blur(90px);
  position: relative;
  z-index: -1;
  left: 2.5rem;
  bottom: -2.5rem;
  grid-row: 2 / span 2;
  align-self: flex-end;
}

@media (min-width: 1024px) {
  .nav-line {
    display: block;
    width: 100%;
    height: 0.5rem;
    background-color: black;
  }

  .section-navigation {
    position: relative;
    // top: calc(-8rem + 2.5rem - 1.5rem);
    width: 100%;
    display: grid;
    grid-template-columns: auto 1fr auto 1fr auto;
    grid-template-rows: 1fr;
    gap: 1rem;
    align-items: center;

    h2 {
      cursor: pointer;
    }
  }

  .content-item {
    display: flex;
    flex-flow: column nowrap;
    row-gap: 2.5rem;
  }
}
</style>
