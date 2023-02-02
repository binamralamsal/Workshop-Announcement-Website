<script>
  import { Idea, Money, Journey, Resources } from "$lib/assets/icons";
  import Button from "$lib/components/Button.svelte";
</script>

<section class="features-section" aria-labelledby="features-title">
  <div class="container features-container even-columns">
    <div class="image" data-aos="fade-right">
      <img src="/home/features-image.jpg" alt="Features" />
    </div>
    <div class="description">
      <header data-aos="fade-left">
        <span class="pre-title color-accent">Who we are</span>
        <h2 class="title" id="features-title">We Offer The Best Carrier</h2>
      </header>

      <ul class="services">
        <li class="service" data-aos="fade-up" data-aos-delay="100">
          <div class="service__icon"><Idea /></div>
          <div class="service__content">
            <h3 class="service__title">Earn Money with Unique Projects</h3>
            <p>
              If a student creates a unique project, we assist them so that they
              can earn money.
            </p>
          </div>
        </li>

        <li class="service" data-aos="fade-up" data-aos-delay="200">
          <div class="service__icon"><Money /></div>
          <div class="service__content">
            <h3 class="service__title">Freelancing for profit</h3>
            <p>
              Learn how to work as a freelancer and make money through our
              instructors.
            </p>
          </div>
        </li>

        <li class="service" data-aos="fade-up" data-aos-delay="300">
          <div class="service__icon"><Journey /></div>
          <div class="service__content">
            <h3 class="service__title">Experience and learn at Journey</h3>
            <p>
              Participate in paid or unpaid internships and receive a
              certificate upon completion.
            </p>
          </div>
        </li>

        <li class="service" data-aos="fade-up" data-aos-delay="400">
          <div class="service__icon"><Resources /></div>
          <div class="service__content">
            <h3 class="service__title">Boost your learning with resources</h3>
            <p>
              Access resources, materials, and quizzes on our Telegram channel
              to enhance your knowledge.
            </p>
          </div>
        </li>
      </ul>
    </div>
  </div>
</section>

<style>
  .features-section {
    padding: 8rem 0;
    overflow: hidden;
    /* background: url("/home/features-bg.jpg"); */
    background-size: cover;
  }

  .features-container {
    gap: 3rem;
    align-items: center;
    position: relative;
  }

  .features-container::before,
  .features-container::after {
    position: absolute;
    right: -20%;
  }

  .features-container::before {
    content: url("/home/features-decoration-1.png");
    top: 10%;
  }

  .features-container::after {
    content: url("/home/features-decoration-2.png");
    bottom: 10%;
  }

  .image {
    position: relative;
  }

  .image img {
    z-index: 20;
    position: relative;
  }

  .image::before,
  .image::after {
    position: absolute;
  }

  .image::before {
    content: url("/home/features-image-1.jpg");
    top: 10%;
    left: -15%;
    z-index: 10;
  }

  .image::after {
    content: url("/home/features-image-2.jpg");
    bottom: 10%;
    right: 0%;
    z-index: 30;
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

  .services {
    margin-top: 2.5rem;
  }

  .services {
    display: flex;
    flex-direction: column;
    gap: 1.875rem;
  }

  .service {
    display: flex;
    gap: 1rem;
  }

  .service__icon {
    align-self: flex-start;
    border-radius: 100%;
    display: flex;
    background: hsla(204, 100%, 55%, 0.1);
    padding: 0.75rem;
  }

  .service__title {
    color: var(--clr-accent-900);
    margin-bottom: 0.3125rem;
    font-size: 1.25rem;
    font-weight: var(--fw-700);
  }

  @media screen and (max-width: 75em) {
    .image::before {
      display: none;
    }
  }

  @media screen and (max-width: 60em) {
    .image::after {
      display: none;
    }
  }

  @media screen and (max-width: 48em) {
    .image img {
      width: 100%;
    }

    .features-container::before,
    .features-container::after {
      display: none;
    }
  }

  @media screen and (max-width: 40em) {
    .features-section {
      padding: 5rem 0;
    }

    .image::before,
    .image::after {
      display: none;
    }
  }
</style>
