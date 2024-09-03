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
    <div class="circle-element circle-1"></div>
    <div class="circle-element circle-2"></div>
    <div class="circle-element circle-3"></div>
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
  background-color: #a770ef;
  left: 50%;
  transform: translateX(-50%);
  bottom: 15rem;
  z-index: -2;
  opacity: 0.95;
}

.circle-2 {
  background-color: #cf8bf3;
  left: 50%;
  transform: translateX(-50%);
  bottom: 5rem;
  z-index: -1;
  opacity: 0.55;
}

.circle-3 {
  background-color: #fdb99b;
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
    left: 2.5%;
    transform: unset;
    bottom: 1rem;
  }

  .circle-2 {
    left: 15%;
    transform: unset;
    bottom: 1rem;
  }

  .circle-3 {
    left: 30%;
    transform: unset;
    bottom: 1rem;
  }
}
</style>
