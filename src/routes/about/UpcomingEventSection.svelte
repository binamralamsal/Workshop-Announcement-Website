<script lang="ts">
  import { onDestroy } from "svelte";

  let deadlineDate = new Date(2023, 1, 20);
  let difference = deadlineDate.getTime() - new Date().getTime();

  const interval = setInterval(() => {
    if (difference <= 0) {
      clearInterval(interval);
      return;
    }
    difference = deadlineDate.getTime() - new Date().getTime();
  }, 1000);

  onDestroy(() => {
    clearInterval(interval);
  });

  $: {
    if (difference <= 0) {
      difference = 0;
    }
  }
</script>

<section class="offers-section" aria-labelledby="events-title">
  <div class="container offers-container">
    <header class="offers-header">
      <h2 class="title" id="offers-title">
        <span class="pre-title " data-aos="fade-up"> Upcoming Event </span>
        <span class="main-title " data-aos="fade-up" data-aos-delay="50">
          Interested in Registering For<span>The Next Event</span>
        </span>
      </h2>
    </header>

    <ul class="countdowns" data-aos="fade-up">
      <li class="countdown">
        <h3 class="countdown-title">
          {Math.floor(difference / (1000 * 60 * 60 * 24))}
        </h3>
        <p class="sub-text">Days</p>
      </li>

      <li class="separator">:</li>

      <li class="countdown">
        <h3 class="countdown-title">
          {Math.floor((difference % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60))}
        </h3>
        <p class="sub-text">Hours</p>
      </li>

      <li class="separator">:</li>

      <li class="countdown">
        <h3 class="countdown-title">
          {Math.floor((difference % (1000 * 60 * 60)) / (1000 * 60))}
        </h3>
        <p class="sub-text">Mins</p>
      </li>

      <li class="separator">:</li>

      <li class="countdown">
        <h3 class="countdown-title">
          {Math.floor((difference % (1000 * 60)) / 1000)}
        </h3>
        <p class="sub-text">Secs</p>
      </li>
    </ul>
  </div>
</section>

<style>
  .offers-section {
    padding: 8rem 0;
    overflow: hidden;
    background: url("/about/upcoming-event-bg.jpg") no-repeat;
    background-size: cover;
    background-position: center;
    color: white;
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

  .countdowns {
    list-style-type: none;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0 auto;
    gap: 1rem;
    flex-wrap: wrap;
    max-width: fit-content;
  }

  .countdown {
    padding: 1rem 1.75rem;
    border-radius: var(--radius-400);
    background: white;
    position: relative;
  }

  .separator {
    font-weight: var(--fw-800);
    font-size: var(--fs-500);
  }

  .countdown-title {
    color: var(--clr-secondary-400);
    font-size: var(--fs-600);
    min-width: 3ch;
    font-weight: var(--fw-700);
  }

  .sub-text {
    color: var(--clr-neutral-300);
    text-transform: uppercase;
    min-width: 6ch;
    font-size: var(--fs-300);
  }

  @media screen and (max-width: 48em) {
    .offers-section {
      padding: 5rem 0;
    }

    .main-title {
      margin-bottom: 2rem;
    }
  }

  @media screen and (max-width: 38em) {
    .separator {
      display: none;
    }
  }
</style>
