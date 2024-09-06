<template>
  <section class="section-grid" id="about-section">
    <div class="section-grid__content">
      <div class="content-item">
        <h1>
          A Little <br />
          About Me
        </h1>
      </div>
    </div>
    <div class="section-grid__content paragraph">
      <div class="content-item">
        <p class="p-1">
          I recently graduated from the Uppsala University in Sweden with a master’s degree in Human
          Computer Interaction. I now strive to be a UX/UI Designer and User Researcher with the
          ambition to be at the forefront of design and technology innovation. <br />
        </p>
        <p class="p-2">
          My education in Human Computer Interaction has made me appreciate user research driven
          design, and has given me the skills for designing user experiences and developing user
          interfaces. It is my passion for design research which has led me with inspiration to
          create truly meaningful and valued user experiences. <br />
        </p>
        <p class="p-3">
          Researching robots and designing for the use of robots in different social contexts is
          also one of my ambitions. I see a certain charm in a future where we can collaborate with
          robots meaningfully, and in doing so can make the world a better place. User Centred
          Design and the field of robotics exist in harmony, in that they both require an extensive
          understanding of the users, of humans. I strive therefore to work in Design to put my
          knowledge to good use, and to explore further the value of interactions within the vast
          realm of Human-Computer Interaction. <br />
        </p>
        <p class="p-4">
          I would like to thank you for taking the time to read my portfolio. I believe that you too
          value Design, and in being where you are now you understand its influence on the world
          we’re in. So let this moment be the beginning of a meaningful collaboration. <br />
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

  .paragraph {
    grid-row: 4;
    align-self: start;
    justify-self: end;

    .content-item {
      display: flex;
      flex-flow: column nowrap;
      row-gap: 5.5rem;

      .p-1,
      .p-2,
      .p-3,
      .p-4 {
        width: 85%;
      }
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
  background-color: #a8ff78;
  left: 50%;
  transform: translateX(calc(-50% - 10%));
  bottom: 4rem;
  z-index: -2;
  opacity: 0.95;
}

.circle-2 {
  background-color: #78ffd6;
  left: 50%;
  transform: translateX(calc(-50% - 5%));
  bottom: 0;
  z-index: -1;
  opacity: 0.55;
}

@media (min-width: 1024px) {
  .section-grid {
    .paragraph {
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
          width: 55%;
        }
      }
    }
  }

  .circle-element {
    width: 550px;
    height: 550px;
    border-radius: 100%;
  }

  .circle-1 {
    left: -5%;
    transform: unset;
    bottom: -1.5rem;
  }

  .circle-2 {
    left: 2.5%;
    transform: unset;
    bottom: -1.5rem;
  }
}
</style>
