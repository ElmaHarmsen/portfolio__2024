<template>
  <section class="section-grid" id="daily-ui-section">
    <div class="section-grid__content bg-colour">
      <div class="subitems-container">
        <router-link to="/experience"><h2>See all work</h2></router-link>
        <span class="nav-line"></span>
      </div>
      <div class="content-item">
        <h2>Daily UI's</h2>
        <div class="content-item__subitems">
          <h2>dropdown</h2>
          <h2>#27</h2>
        </div>
      </div>
    </div>
    <div class="section-grid image-grid">
      <img
        class="content-item__image"
        src="../assets/imgs/DailyUI27.png"
        alt="Daily UI #27 Gradient picker dropdown"
      />
      <img class="content-item__image" src="../assets//imgs/unsplash-img-1.jpg" alt="" />
    </div>
  </section>
</template>

<style lang="scss" scoped>
.bg-colour {
  background-color: aquamarine;
}

.content-item {
  display: flex;
  flex-flow: row nowrap;
  justify-content: space-between;
  column-gap: 5rem;

  &__subitems {
    display: flex;
    flex-flow: row nowrap;
    column-gap: 5rem;
  }

  &__image {
    width: 100%;
  }
}
</style>
