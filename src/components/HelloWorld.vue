<template>
  <section class="landing-grid">
    <div class="landing-grid__content">
      <div class="content-item">
        <h1>Embracing Design for Humans, Robots & AI</h1>
        <div class="subitems-container">
          <h2>Elma Harmsen</h2>
          <h2>
            UI/UX Designer & <br class="phone-only" />
            User Researcher
          </h2>
        </div>
      </div>
    </div>
    <div class="circle-element circle-1"></div>
    <div class="circle-element circle-2"></div>
  </section>
</template>

<style lang="scss" scoped>
.circle-element {
  width: 350px;
  height: 350px;
  border-radius: 100%;
  position: absolute;
}

.circle-1 {
  background-color: #d4fc79;
  left: 50%;
  transform: translateX(-50%);
  bottom: 15rem;
  z-index: -2;
  opacity: 0.95;
}

.circle-2 {
  background-color: #96e6a1;
  left: 50%;
  transform: translateX(-50%);
  bottom: 5rem;
  z-index: -1;
  opacity: 0.55;
}

@media (min-width: 1024px) {
  .circle-element {
    width: 600px;
    height: 600px;
    border-radius: 100%;
  }

  .circle-1 {
    left: 50%;
    transform: translateX(-75%);
    bottom: 2.5rem;
  }

  .circle-2 {
    left: 50%;
    transform: translateX(-50%);
    bottom: 1rem;
  }
}
</style>
