<script>
  import Button from "$lib/components/Button.svelte";
</script>

<section class="about-section" aria-labelledby="about-title">
  <div class="container about-container even-columns">
    <div class="images">
      <div class="row-1">
        <div class="row__image-1-container" data-aos="fade-right">
          <div class="row__icon">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="icon icon-tabler icon-tabler-medal"
              width="26"
              height="26"
              viewBox="0 0 24 24"
              stroke-width="2"
              stroke="currentColor"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
            >
              <path stroke="none" d="M0 0h24v24H0z" fill="none" />
              <path d="M12 4v3m-4 -3v6m8 -6v6" />
              <path
                d="M12 18.5l-3 1.5l.5 -3.5l-2 -2l3 -.5l1.5 -3l1.5 3l3 .5l-2 2l.5 3.5z"
              />
            </svg>
          </div>
          <img src="/home/about-image-1.jpg" class="image-1" alt="" />
        </div>
        <img
          src="/home/about-image-2.jpg"
          class="image-2"
          alt=""
          data-aos="fade-right"
        />
      </div>
      <div class="row-2" data-aos="fade-right" data-aos-delay="150">
        <div class="students-count">
          <div class="count__icon">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="icon icon-tabler icon-tabler-mood-happy"
              width="24"
              height="24"
              viewBox="0 0 24 24"
              stroke-width="2"
              stroke="currentColor"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
            >
              <path stroke="none" d="M0 0h24v24H0z" fill="none" />
              <circle cx="12" cy="12" r="9" />
              <line x1="9" y1="9" x2="9.01" y2="9" />
              <line x1="15" y1="9" x2="15.01" y2="9" />
              <path d="M8 13a4 4 0 1 0 8 0m0 0h-8" />
            </svg>
          </div>

          <div class="count__content">
            <h3 class="count__title">12</h3>
            <p class="count__description">Interesting Courses</p>
          </div>
        </div>
        <img src="/home/about-image-3.jpg" class="image-3" alt="" />
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
          Creating A Community Of Life Long Learners
        </h2>
      </header>

      <p class="caption" data-aos="fade-up" data-aos-delay="300">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec nunc null
        liobortis nibh porttitor. Facilisi arcu, nibh vel risus, morbi pharetra.
        Facilisi sit miam mauris non iaculis elit fusce amet nunc in odio
        molestie.
      </p>

      <div class="features even-columns">
        <div class="feature">
          <div class="feature__icon" data-aos="fade-up" data-aos-delay="450">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="icon icon-tabler icon-tabler-device-laptop"
              width="30"
              height="30"
              viewBox="0 0 24 24"
              stroke-width="2"
              stroke="currentColor"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
            >
              <path stroke="none" d="M0 0h24v24H0z" fill="none" />
              <line x1="3" y1="19" x2="21" y2="19" />
              <rect x="5" y="6" width="14" height="10" rx="1" />
            </svg>
          </div>

          <div class="feature__content">
            <h3 class="feature__title" data-aos="fade-up" data-aos-delay="450">
              Flexible Classes
            </h3>
            <p
              class="feature__description"
              data-aos="fade-up"
              data-aos-delay="600"
            >
              There are many variations of passages of the Ipsum available for
              now
            </p>
          </div>
        </div>

        <div class="feature">
          <div class="feature__icon" data-aos="fade-up" data-aos-delay="450">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="icon icon-tabler icon-tabler-school"
              width="30"
              height="30"
              viewBox="0 0 24 24"
              stroke-width="2"
              stroke="currentColor"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
            >
              <path stroke="none" d="M0 0h24v24H0z" fill="none" />
              <path d="M22 9l-10 -4l-10 4l10 4l10 -4v6" />
              <path d="M6 10.6v5.4a6 3 0 0 0 12 0v-5.4" />
            </svg>
          </div>

          <div class="feature__content">
            <h2 class="feature__title" data-aos="fade-up" data-aos-delay="450">
              Educator Support
            </h2>
            <p class="feature__caption" data-aos="fade-up" data-aos-delay="600">
              There are many variations of passages of the Ipsum available for
              now
            </p>
          </div>
        </div>
      </div>

      <div data-aos="fade-up" data-aos-delay="700">
        <Button href="/about">
          <span> Learn More </span>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="icon icon-tabler icon-tabler-arrow-right"
            width="18"
            height="18"
            viewBox="0 0 24 24"
            stroke-width="2"
            stroke="currentColor"
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
            <line x1="5" y1="12" x2="19" y2="12" />
            <line x1="13" y1="18" x2="19" y2="12" />
            <line x1="13" y1="6" x2="19" y2="12" />
          </svg>
        </Button>
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

  .images {
    display: flex;
    flex-direction: column;
    align-items: center;
    position: relative;
    padding: 1rem;
    gap: 1rem;
  }

  .images::before,
  .images::after {
    position: absolute;
    left: -50%;
  }

  .images::before {
    content: url("/home/about-shape-1.png");
    top: -10%;
  }

  .images::after {
    content: url("/home/about-shape-3.png");
    bottom: -10%;
  }

  .about-description {
    position: relative;
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

  .row-1 {
    display: flex;
    gap: 1rem;
  }

  .row__image-1-container {
    align-self: flex-end;
    justify-self: flex-end;
    display: flex;
    justify-content: center;
    position: relative;
  }

  .row__icon {
    z-index: 999;
    padding: 0.75rem;
    border-radius: 100%;
    position: absolute;
    display: flex;
    top: -1.5rem;
    justify-content: center;
    align-items: center;
    background: var(--clr-accent-400);
    color: white;
  }

  .image-2 {
    align-self: flex-start;
    justify-self: flex-end;
  }

  .row-2 {
    position: relative;
  }

  .students-count {
    padding: 1rem;
    display: flex;
    background: white;
    top: 50%;
    left: -25px;
    gap: 0.75rem;
    position: absolute;
    box-shadow: 0 10px 25px rgb(0 0 0 / 8%);
    border-radius: var(--radius-600);
    align-items: center;
    animation: bounceSlide 4s infinite;
  }

  @keyframes bounceSlide {
    0%,
    20%,
    50%,
    80%,
    100% {
      transform: translateY(0);
    }
    40% {
      transform: translateY(-30px);
    }
    60% {
      transform: translateY(-15px);
    }
  }

  .count__icon {
    padding: 0.75em;
    background: var(--clr-accent-400);
    border-radius: 100%;
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .count__title {
    font-weight: var(--fw-700);
    color: var(--clr-accent-400);
  }

  .caption {
    margin: 1.875rem 0;
  }

  .features {
    gap: 1rem;
    margin-bottom: 2rem;
  }

  .feature {
    display: flex;
    gap: 1rem;
    align-items: flex-start;
  }

  .feature__icon {
    padding: 0.75em;
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    background: var(--clr-accent-400);
    border-radius: 100%;
  }

  .feature__title {
    color: var(--clr-accent-900);
    font-size: var(--fs-500);
    font-weight: var(--fw-600);
    margin-bottom: 0.625rem;
  }

  @media screen and (max-width: 68em) {
    .image-1 {
      height: 180px;
    }

    .image-2 {
      height: 230px;
    }

    .image-3 {
      height: 150px;
    }
  }

  @media screen and (max-width: 60em) {
    .features {
      grid-template-columns: 1fr;
    }
  }

  @media screen and (max-width: 56em) {
    .image-1 {
      height: 140px;
    }

    .image-2 {
      height: 190px;
    }

    .image-3 {
      height: 110px;
    }
  }

  @media screen and (max-width: 48em) {
    .about-section {
      padding: 3rem 0;
    }

    .images {
      padding: 0 3rem;
    }

    .images::before,
    .images::after,
    .about-description::before,
    .about-description::after {
      display: none;
    }

    .image-1,
    .row__image-1-container,
    .image-2,
    .image-3 {
      width: 100%;
      height: auto;
    }

    .students-count {
      bottom: 0.5rem;
      left: 0.5rem;
      top: auto;
    }
  }

  @media screen and (max-width: 40em) {
    .row-1,
    .row-2 {
      flex-direction: column;
      width: 100%;
    }
  }

  @media screen and (max-width: 30em) {
    .images {
      padding: 0;
    }
  }
</style>
