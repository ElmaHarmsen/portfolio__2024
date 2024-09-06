<template>
  <section class="section-grid" id="ux-project-section">
    <div class="section-grid__content">
      <div class="content-item">
        <h1>
          The UX <br />
          Case
        </h1>
      </div>
    </div>
    <div class="section-grid__content container">
      <div class="content-item">
        <p class="p-1">
          This UX project was conducted a team endeavour as part of my studies in Human Computer
          Interaction at the Uppsala University. The project’s objective was to design a system that
          could support sustainability and reduce waste in fast fashion. <br />
        </p>
        <p class="p-2">
          Producing fashion costs thousands of litres of water and other natural resources, and
          results in millions of tonnes of waste on landfills every year. The environmental impact
          of fast fashion is substantial, and the problem of fast fashion is one affecting everyone.
          Yet, not enough is done to achieve reusability of clothes, which is exactly the issue that
          this project sought to solve. <br />
        </p>
        <p class="p-3">
          The project evolved in different stages, staring with ideating, in which different
          ideation methods were used to brainstorm ideas that could evolve into concepts. The
          concepts were created using low fidelity wireframes, where we decided to allow all members
          of the team to design her concept and express her thought behind the design process. After
          some extensive deliberations and short evaluations of the concepts, we continued with just
          one, where we combined our skills to design a high fidelity prototype in Figma. Following
          this stage came one that involved thorough evaluations with multiple users, as well as
          iterations on the design where improvements were necessary. <br />
        </p>
      </div>
      <div class="content-item image-grid">
        <div class="container">
          <img
            class="content-item__image"
            src="../assets/imgs/ux-project-3.png"
            alt="UX project app screenshot profile page"
          />
          <h2>Profile page</h2>
        </div>
        <div class="container">
          <img
            class="content-item__image"
            src="../assets/imgs/ux-project-2.png"
            alt="UX project app screenshot homepage with events"
          />
          <h2>Events page</h2>
        </div>
        <div class="container">
          <img
            class="content-item__image"
            src="../assets/imgs/ux-project-1.png"
            alt="UX project app screenshot environmental impact infographic"
          />
          <h2>Infographic</h2>
        </div>
      </div>
      <div class="content-item">
        <p class="p-4">
          Results of the project were positive as users expressed feelings of happiness and
          satisfaction with the idea of using the clothing swap solution in their nearby community.
          To us, the design team, it felt important to know that we tool sufficient time to research
          the problem, brainstorm potential solutions and evaluate multiple possibilities, but
          equally so to realise the value of design when it comes to the encouragement of making
          sustainable, yet fashionalbe choices. <br />
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

    .content-item {
      display: flex;
      flex-flow: column nowrap;
      row-gap: 5.5rem;

      .p-1,
      .p-2,
      .p-3,
      .p-4 {
        width: 80%;
      }

      &__image {
        width: 70%;
      }

      .container {
        display: flex;
        flex-flow: column nowrap;
        row-gap: 1rem;
      }
    }

    .image-grid {
      display: flex;
      flex-flow: column wrap;
    }
  }
  .container {
    grid-row: 4;
    display: flex;
    flex-flow: column nowrap;
    row-gap: 8rem;
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
  background-color: #649173;
  left: 50%;
  transform: translateX(calc(-50% - 10%));
  bottom: 4rem;
  z-index: -2;
  opacity: 0.95;
}

.circle-2 {
  background-color: #dbd5a4;
  left: 50%;
  transform: translateX(calc(-50% - 5%));
  bottom: 0;
  z-index: -1;
  opacity: 0.55;
}

@media (min-width: 1024px) {
  .section-grid {
    &__content {
      .content-item {
        row-gap: 8rem;

        .p-1 {
          width: 75%;
        }
        .p-2 {
          width: 40%;
        }
        .p-3 {
          width: 50%;
        }
        .p-4 {
          width: 35%;
        }

        &__image {
          width: 350px;
        }
      }

      .image-grid {
        flex-flow: row wrap;
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
