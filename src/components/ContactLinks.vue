<template>
  <section class="footer-grid">
    <div class="footer-grid__content">
      <div class="content-item">
        <img class="figure-image" src="../assets/imgs/footer-figure.png" alt="" />
        <img class="figure-image" src="../assets/imgs/footer-figure-2.png" alt="" />
        <img class="figure-image" src="../assets/imgs/footer-figure-3.png" alt="" />
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.line-image {
  width: 30px;
  transform: translateX(-50px) translateY(10px);
  position: absolute;
}

.figure-image {
  width: 100px;
}

.footer-grid {
  display: grid;
  grid-template-columns: 35% 1fr 5%;
  grid-template-rows: 200px 1fr 100px;

  &__content {
    grid-column: 2;
    grid-row-start: 2;
  }

  .content-item {
    display: flex;
    flex-flow: row nowrap;
    column-gap: 50px;
    height: 100%;
  }
}
</style>
