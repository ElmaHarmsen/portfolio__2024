<template>
  <section class="landing-grid">
    <div class="landing-grid__content">
      <div class="content-item">
        <h1>
          Designing <br />
          Human-Centred
        </h1>
        <div class="subitems-container">
          <h2>Selection of recent work</h2>
        </div>
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
  width: 400px;
  height: 400px;
  border-radius: 300px 250px 300px 250px;
  filter: blur(70px);
  position: absolute;
  z-index: -1;
  bottom: 5.5rem;
  left: 1%;
}

@media (min-width: 1024px) {
  .circle-element {
    width: 600px;
    height: 600px;
    border-radius: 300px 400px 300px 400px;
    filter: blur(90px);
    bottom: 1.5rem;
    left: 20%;
  }
}
</style>
