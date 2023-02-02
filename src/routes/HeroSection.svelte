<script>
  import Button from "$lib/components/Button.svelte";
</script>

<section aria-labelledby="hero-title" class="hero-section">
  <div class="container hero-container even-columns">
    <div>
      <header>
        <span class="pre-title color-accent" data-aos="fade-up"
          >Better learning future with us</span
        >
        <h1
          class="title"
          data-aos="fade-up"
          data-aos-delay="150"
          id="hero-title"
        >
          Committed To Learn Excellence In Education
        </h1>
      </header>
      <p class="caption" data-aos="fade-up" data-aos-delay="300">
        It is long established that a reader will be distracted by the readable
        popular and best content.
      </p>

      <div data-aos="fade-up" data-aos-delay="450">
        <Button href="/course-details">
          <span> Learn More </span>
          <svg
            class="icon icon-tabler icon-tabler-arrow-right"
            fill="none"
            height="18"
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            viewBox="0 0 24 24"
            width="18"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path d="M0 0h24v24H0z" fill="none" stroke="none" />
            <line x1="5" x2="19" y1="12" y2="12" />
            <line x1="13" x2="19" y1="18" y2="12" />
            <line x1="13" x2="19" y1="6" y2="12" />
          </svg>
        </Button>
      </div>
    </div>
    <div class="right-images">
      <img
        alt="Girl thumbchecking"
        class="girl-image"
        data-aos="fade-left"
        data-aos-delay="450"
        height="854"
        src="/home/girl-thumb.png"
      />
      <img
        alt="Girl background"
        class="girl-bg"
        data-aos="fade-left"
        data-aos-delay="600"
        src="/home/girl-bg.png"
      />
    </div>
  </div>

  <div class="decorations">
    <img alt="Decoration 1" class="shape-1" src="/home/shape-1.png" />
    <img alt="Decoration 3" class="shape-3" src="/home/shape-3.png" />
  </div>
</section>

<style>
  .hero-section {
    background: url("/home/hero-background.jpg") no-repeat;
    background-size: cover;
  }

  .hero-container {
    padding: 12rem 0 10rem 0;
    position: relative;
  }

  .pre-title {
    font-weight: var(--fw-700);
    display: flex;
    align-items: center;
    gap: 0.5em;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    margin-bottom: 0.625rem;
  }

  .pre-title::before {
    content: "";
    height: 0.15em;
    background: var(--clr-accent-400);
    width: 3.125em;
  }

  .title {
    font-size: var(--fs-900);
    font-weight: var(--fw-800);
    color: var(--clr-accent-900);
    line-height: 1.25;
    max-width: 15ch;
  }

  .caption {
    font-size: var(--fs-500);
    line-height: 2em;
    margin: 1.875rem 0;
    max-width: 45ch;
  }

  .girl-bg,
  .girl-image {
    position: absolute;
    right: 0;
    bottom: 0;
    height: 80%;
  }

  .girl-bg {
    height: 65%;
  }

  .girl-image {
    z-index: 99;
  }

  .right-images::before {
    content: url("/home/shape-2.png");
    position: relative;
    top: 0;
    left: 0;
  }

  .shape-1,
  .shape-3 {
    position: absolute;
  }

  .shape-1 {
    left: 10px;
    top: 90px;
  }

  .shape-3 {
    top: 250px;
    right: 5%;
  }

  @media screen and (max-width: 68em) {
    .shape-1 {
      display: none;
    }

    .girl-image {
      height: 60%;
    }

    .girl-bg {
      height: 50%;
    }
  }

  @media screen and (max-width: 56.25em) {
    .hero-container {
      grid-template-columns: 1fr;
      padding: 8rem 0 6rem 0;
    }

    .title,
    .caption {
      max-width: 100%;
    }

    .girl-image,
    .girl-bg,
    .shape-1,
    .shape-3,
    .right-images::before {
      display: none;
    }
  }
</style>
