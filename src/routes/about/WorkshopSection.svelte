<script>
  import Button from "$lib/components/Button.svelte";
</script>

<section class="workshop-section" aria-labelledby="workshop-title">
  <div class="container workshop-container even-columns">
    <div class="description">
      <header data-aos="fade-right">
        <span class="pre-title">Free Workshop</span>
        <h2 class="title" id="workshop-title">Join Our Free Workshops</h2>
      </header>
      <p class="workshop-detail" data-aos="fade-right">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sit amet,
        consect adipi scing elit, sed do eiusmod tempor incididunt ut sed do
        eiusmod tempor incididunt ut labore et dolore aliqua.
      </p>

      <div data-aos="fade-right">
        <Button variant="light-secondary" size="large" href="/course-details">
          <span>Join Event</span>
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

    <div class="workshop-image" data-aos="fade-left">
      <img src="/about/workshop.jpg" alt="workshop" />
    </div>
  </div>
</section>

<style>
  .workshop-section {
    padding: 8rem 0;
    overflow: hidden;
    background-size: cover;
    background: url("/about/workshop-bg.png"), var(--clr-accent-400);
    color: white;
  }

  .workshop-container {
    gap: 3rem;
    align-items: center;
    position: relative;
  }

  .workshop-detail {
    margin: 2.5rem 0;
  }

  .workshop-image {
    position: relative;
  }

  .workshop-image img {
    z-index: 99;
    position: relative;
  }

  .workshop-image::before {
    content: url("/about/workshop-01.png");
    position: absolute;
    bottom: -15%;
    right: -10%;
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
    line-height: 1.4;
  }

  @media screen and (max-width: 48em) {
    .workshop-container::after {
      display: none;
    }
  }

  @media screen and (max-width: 40em) {
    .workshop-section {
      padding: 5rem 0;
    }
  }
</style>
