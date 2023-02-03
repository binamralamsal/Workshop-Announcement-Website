<section class="about-section" aria-labelledby="about-title">
  <div class="container about-container even-columns">
    <div class="images" data-aos-delay="50" data-aos="fade-right">
      <div class="session-stats">
        <strong class="stat-title color-accent">2.98</strong>
        <p class="stat-details color-heading">Finished Session</p>
      </div>
      <img src="/about/about.png" alt="About" />

      <div class="about-bottom-image">
        <img src="/about/about-image-bottom.png" class="main" alt="" />
        <div class="circle-image" />
      </div>
    </div>
    <div class="about-description">
      <header>
        <span class="pre-title color-accent" data-aos="fade-up">About us</span>
        <h2
          class="title"
          id="about-title"
          data-aos="fade-up"
          data-aos-delay="150"
        >
          Knowledge is power, Information is liberating.
        </h2>
      </header>

      <p class="caption" data-aos="fade-up" data-aos-delay="300">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Amet, venenatis
        dictum et nec. Fringilla dictum tristique cras pellentesque consequat.
      </p>

      <h3
        class="features-title color-heading"
        data-aos="fade-up"
        data-aos-delay="400"
      >
        People Love To Learn With us
      </h3>

      <div
        class="features even-columns"
        data-aos="fade-up"
        data-aos-delay="500"
      >
        <div class="feature">
          <h4 class="feature-stat">90%</h4>
          <div class="feature__content">
            <p class="feature__description">
              90% of students see their course through to completion.
            </p>
          </div>
        </div>

        <div class="feature">
          <h4 class="feature-stat" data-aos="fade-up">9/10</h4>
          <div class="feature__content">
            <p class="feature__description">
              9/10 users reported better learning outcomes.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<style>
  .about-section {
    padding: 8rem 0;
    overflow: hidden;
  }

  .about-container {
    align-items: center;
    gap: 3rem;
  }

  .pre-title {
    font-weight: var(--fw-700);
    text-transform: uppercase;
    letter-spacing: 0.1em;
    margin-bottom: 0.625rem;
    display: block;
  }

  .title {
    font-size: var(--fs-700);
    font-weight: var(--fw-800);
    color: var(--clr-heading);
    line-height: 1.4;
  }

  .about-description {
    position: relative;
  }

  .images {
    position: relative;
  }

  .about-bottom-image {
    position: absolute;
    width: 50%;
    bottom: -10%;
    right: 0;
  }

  .about-bottom-image .main {
    position: relative;
    z-index: 2;
  }

  .circle-image {
    width: 100%;
    position: absolute;
    bottom: -2%;
    right: -5%;
    height: 100%;
    border-radius: 38% 62% 64% 36%/43% 35% 65% 57%;
    border: 2px solid var(--clr-secondary-400);
    animation: rotate-animate 13s linear infinite;
  }

  .session-stats {
    position: absolute;
    top: 5%;
    left: -15%;
    background: white;
    border-radius: 100%;
    padding: 2rem;
    aspect-ratio: 1/1;
    box-shadow: 0 10px 35px rgb(0 0 0 / 5%);
    display: flex;
    flex-direction: column;
    justify-content: center;
    text-align: center;
    align-items: center;
  }

  .stat-title {
    font-size: var(--fs-600);
    font-weight: var(--fw-700);
  }

  .stat-details {
    font-weight: var(--fw-700);
    max-width: 10ch;
  }

  @keyframes rotate-animate {
    0% {
      transform: rotate(0deg);
    }
    to {
      transform: rotate(1turn);
    }
  }

  @media screen and (max-width: 48em) {
    .about-bottom-image {
      display: none;
    }

    .session-stats {
      top: 0;
      left: 0;
      padding: 1rem;
    }
  }

  .about-description::before,
  .about-description::after {
    position: absolute;
    right: -50%;
  }

  .about-description::before {
    content: url("/home/about-shape-2.png");
    top: -10%;
  }

  .about-description::after {
    content: url("/home/about-shape-4.png");
    bottom: -10%;
  }

  .caption {
    margin: 1.875rem 0;
  }

  .features-title {
    margin-bottom: 1.25rem;
    font-weight: var(--fw-700);
    font-size: 1.25rem;
  }

  .feature-stat {
    font-size: var(--fs-600);
    font-weight: var(--fw-700);
    color: var(--clr-secondary-400);
    margin-bottom: 0.3125rem;
  }

  .features {
    gap: 1rem;
    margin-bottom: 2rem;
  }

  @media screen and (max-width: 60em) {
    .features {
      grid-template-columns: 1fr;
    }
  }

  @media screen and (max-width: 48em) {
    .about-section {
      padding: 3rem 0;
    }
  }
</style>
