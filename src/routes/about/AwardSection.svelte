<section class="award-section" aria-labelledby="events-title">
  <div class="container award-container">
    <header class="award-header">
      <h2 class="title" id="award-title">
        <span class="pre-title color-accent" data-aos="fade-up"> Award </span>
        <span
          class="main-title color-heading"
          data-aos="fade-up"
          data-aos-delay="50"
        >
          Our Winning Award
        </span>
      </h2>
    </header>

    <ul class="awards">
      <li class="award" data-aos="fade-up">
        <img src="/about/award-01.png" alt="" class="award-image" />
        <p class="award-sub-text">Market / 2023</p>
        <h3 class="award-title color-heading">Evanto Design of The Week</h3>
      </li>

      <li class="award" data-aos="fade-up">
        <img src="/about/award-02.png" alt="" class="award-image" />
        <p class="award-sub-text">Udemy / 2023</p>
        <h3 class="award-title color-heading">Award Site of The Year</h3>
      </li>

      <li class="award" data-aos="fade-up">
        <img src="/about/award-03.png" alt="" class="award-image" />
        <p class="award-sub-text">Review / 2023</p>
        <h3 class="award-title color-heading">Best Customer Support</h3>
      </li>

      <li class="award" data-aos="fade-up">
        <img src="/about/award-04.png" alt="" class="award-image" />
        <p class="award-sub-text">Market / 2023</p>
        <h3 class="award-title color-heading">Top Selling Premium Item</h3>
      </li>
    </ul>
  </div>
</section>

<style>
  .award-section {
    padding: 8rem 0;
    overflow: hidden;
  }

  .award-container {
    text-align: center;
    position: relative;
  }

  .title span {
    display: block;
  }

  .pre-title {
    font-weight: var(--fw-700);
    text-transform: uppercase;
    margin-bottom: 0.3125rem;
  }

  .main-title {
    font-size: var(--fs-700);
    font-weight: var(--fw-800);
    line-height: 1.4;
    margin-bottom: 3.125rem;
  }

  .awards {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
    list-style-type: none;
    position: relative;
  }

  .awards::before {
    content: url("/about/award-decoration.png");
    position: absolute;
    top: -20%;
    right: -5%;
  }

  .award {
    border-radius: var(--radius-400);
    padding: 2.5rem;
    display: grid;
    place-items: center;
    background: white;
    text-align: center;
    box-shadow: 0 10px 30px rgb(0 0 0 / 6%);
    transition: 0.4s 0s;
  }

  .award:hover {
    transform: translateY(-1rem);
  }

  .award:hover .award-title {
    color: var(--clr-accent-400);
  }

  .award-image {
    margin-bottom: 1.875rem;
  }

  .award-sub-text {
    font-size: var(--fs-300);
    font-weight: var(--fw-600);
    color: var(--clr-neutral-300);
  }

  .award-title {
    font-size: var(--fs-500);
    transition: 0.4s;
    font-weight: var(--fw-700);
  }

  @media screen and (max-width: 60em) {
    .awards {
      grid-template-columns: repeat(3, 1fr);
    }
  }

  @media screen and (max-width: 48em) {
    .award-section {
      padding: 5rem 0;
    }

    .main-title {
      margin-bottom: 2rem;
    }

    .awards {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media screen and (max-width: 32em) {
    .awards {
      grid-template-columns: repeat(1, 1fr);
    }
  }
</style>
