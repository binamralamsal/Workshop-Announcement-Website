<section class="offers-section" aria-labelledby="events-title">
  <div class="container offers-container">
    <header class="offers-header">
      <h2 class="title" id="offers-title">
        <span class="pre-title color-accent" data-aos="fade-up">
          What We Offer
        </span>
        <span
          class="main-title color-heading"
          data-aos="fade-up"
          data-aos-delay="50"
        >
          Learn New Skills When And<span>Where You Like</span>
        </span>
      </h2>
    </header>

    <ul class="offers">
      <li class="offer offer-01" data-aos="fade-up" data-aos-delay="100">
        <div class="offer-icon">
          <img src="/about/offer-01.png" alt="" />
        </div>
        <h3 class="offer-title">Remote Learning</h3>
        <p class="offer-description">
          Lorem Ipsum is simply dummy text of the printing and typesetting
          industry.
        </p>
      </li>

      <li class="offer offer-02" data-aos="fade-up" data-aos-delay="200">
        <div class="offer-icon">
          <img src="/about/offer-02.png" alt="" />
        </div>
        <h3 class="offer-title">Awesome Tutors</h3>
        <p class="offer-description">
          Lorem Ipsum is simply dummy text of the printing and typesetting
          industry.
        </p>
      </li>

      <li class="offer offer-03" data-aos="fade-up" data-aos-delay="300">
        <div class="offer-icon">
          <img src="/about/offer-03.png" alt="" />
        </div>
        <h3 class="offer-title">Global Certificate</h3>
        <p class="offer-description">
          Lorem Ipsum is simply dummy text of the printing and typesetting
          industry.
        </p>
      </li>

      <li class="offer offer-04" data-aos="fade-up" data-aos-delay="400">
        <div class="offer-icon">
          <img src="/about/offer-04.png" alt="" />
        </div>
        <h3 class="offer-title">Carrier Guideline</h3>
        <p class="offer-description">
          Lorem Ipsum is simply dummy text of the printing and typesetting
          industry.
        </p>
      </li>
    </ul>
  </div>
</section>

<style>
  .offers-section {
    padding: 1rem 0 8rem 0;
    overflow: hidden;
  }

  .offers-container {
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
    margin-bottom: 3.5rem;
  }

  .offers {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 1.875rem;
    position: relative;
    list-style-type: none;
  }

  .offer {
    padding: 2.5rem 1.875rem;
    border-radius: 0.3125rem;
    display: grid;
    place-items: center;
  }

  .offer-icon {
    margin-bottom: 1.6rem;
    padding: 1.25rem;
    background: white;
    border-radius: 100%;
    display: flex;
  }

  .offer-title {
    font-size: 1.2rem;
    font-weight: var(--fw-700);
    margin-bottom: 1rem;
  }

  .offer-01 {
    background: hsl(171, 50%, 95%);
  }

  .offer-02 {
    background: hsl(18, 100%, 97%);
  }

  .offer-03 {
    background: hsl(217, 68%, 96%);
  }

  .offer-04 {
    background: hsl(0, 100%, 97%);
  }

  .offers::before,
  .offers::after {
    position: absolute;
  }

  .offers::before {
    content: url("/home/events-decoration-1.png");
    right: -4%;
    top: -6%;
  }

  .offers::after {
    content: url("/home/events-decoration-2.png");
    right: -10%;
    bottom: -10%;
  }

  @media screen and (max-width: 64em) {
    .offers {
      grid-template-columns: repeat(3, 1fr);
    }
  }

  @media screen and (max-width: 48em) {
    .offers-section {
      padding: 1rem 0 5rem 0;
    }

    .main-title {
      margin-bottom: 2rem;
    }

    .offers::before,
    .offers::after {
      display: none;
    }

    .offers {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media screen and (max-width: 40em) {
    .offers {
      grid-template-columns: 1fr;
    }
  }
</style>
