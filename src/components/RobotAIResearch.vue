<template>
  <section class="section-grid" id="research-section">
    <div class="section-grid__content">
      <div class="content-item">
        <h1>
          Robot-AI <br />
          Research
        </h1>
      </div>
    </div>
    <div class="section-grid__content container">
      <div class="content-item">
        <p class="p-1">
          The objective of my master thesis from my studies in Human Computer Interaction was to
          research the purpose of robots and Artificial Intelligence in work environments, and seek
          an understanding of their potential role in the future. In doing this research I have
          found the value and delight that research of this kind can offer, as it inspired great
          deliberations and thought provoking discussions on the meaning of humans, robots, AI and
          technology. <br />
        </p>
      </div>
      <div class="content-item image-grid">
        <img
          class="content-item__image"
          src="../assets/imgs/RobotScene1.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
        <img
          class="content-item__image"
          src="../assets/imgs/RobotScene3.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
        <img
          class="content-item__image"
          src="../assets/imgs/RobotScene4.png"
          alt="Daily UI #27 Gradient picker dropdown"
        />
      </div>
      <div class="content-item">
        <p class="p-2">
          The discussions that followed involved the questioning of the definitions on Artificial
          Intelligence and robots, and the evaluation of what it means for technology to actually be
          artificial as opposed to being human. It was inspiring to discuss what this definition
          means for the collaboration between humans and AI, and how this influences any potential
          risks that accompany this collaboration. <br />
        </p>
        <p class="p-3">
          I believe it to be of great importance to research the role and placement of technology in
          our society, because introducing technology of any kind, especially Artificial
          Intelligence and robotics, can greatly influence the way we define ourselves, our role and
          our purpose in the workplace. My ambition is to be at the forefront of research and design
          in social robotics and AI, to explore the possibilities and ethical complications with
          interactions between humans and robots, and to help society thrive forward. <br />
        </p>
      </div>
    </div>
    <!-- <div class="circle-element circle-1"></div>
    <div class="circle-element circle-2"></div> -->
  </section>
</template>

<style lang="scss" scoped>
.section-grid {
  grid-template-rows: 8rem calc(100vh - (2 * 8rem)) 8rem 1fr 8rem;

  &__content {
    align-self: flex-end;
  }

  .container {
    grid-row: 4;
    row-gap: 8rem;

    .content-item {
      display: flex;
      flex-flow: column nowrap;
      row-gap: 8rem;

      .p-1,
      .p-2,
      .p-3 {
        width: 80%;
      }

      &__image {
        width: 100%;
        border: 0.5rem solid black;
      }
    }

    .image-grid {
      display: grid;
      grid-template-columns: 1fr;
      grid-template-rows: 1fr 1fr 1fr;
      gap: 2.5rem;
    }
  }
}

.circle-element {
  opacity: 0.95;
  width: 350px;
  height: 350px;
  border-radius: 100%;
  position: relative;
  grid-row: 2 / span 2;
  grid-column: 2;
  align-self: flex-end;
}

.circle-1 {
  background-color: #e3eeff;
  left: 50%;
  transform: translateX(calc(-50% - 10%));
  bottom: 4rem;
  z-index: -2;
  opacity: 0.55;
}

.circle-2 {
  background-color: #f3e7e9;
  left: 50%;
  transform: translateX(calc(-50% - 5%));
  bottom: 0;
  z-index: -1;
  opacity: 0.55;
}

@media (min-width: 1024px) {
  .section-grid {
    .container {
      .content-item {
        row-gap: 8rem;

        .p-1 {
          width: 60%;
        }
        .p-2 {
          width: 85%;
        }
        .p-3 {
          width: 45%;
        }
      }

      .image-grid {
        grid-template-columns: 1fr 1fr 1fr;
        grid-template-rows: 1fr;
        gap: 1rem;
      }
    }
  }

  .circle-element {
    width: 550px;
    height: 550px;
    border-radius: 100%;
  }

  .circle-1 {
    left: -10%;
    transform: unset;
    bottom: -1rem;
  }

  .circle-2 {
    left: -5%;
    transform: unset;
    bottom: -1.5rem;
  }
}
</style>
