<script>
  import Button from "$lib/components/Button.svelte";
  import CourseCard from "$lib/components/CourseCard.svelte";
</script>

<section class="courses-section" aria-labelledby="courses-title">
  <div class="container courses-container">
    <header class="courses-header">
      <h2 class="title" id="courses-title">
        <span class="pre-title color-accent" data-aos="fade-up"
          >Popular Courses</span
        >
        <span
          class="main-title color-heading"
          data-aos="fade-up"
          data-aos-delay="50">Featured On This Month</span
        >
      </h2>
    </header>

    <div class="even-columns courses-cards">
      <CourseCard
        course={{
          duration: "2 weeks",
          image: {
            alt: "Course",
            src: "/courses/course-01.jpg",
          },
          numberOfModules: 20,
          title: "Complete Typescript course",
        }}
        data-aos="fade-up"
        data-aos-delay="100"
      />
      <CourseCard
        course={{
          duration: "2 weeks",
          image: {
            alt: "Course",
            src: "/courses/course-02.jpg",
          },
          numberOfModules: 20,
          title: "Complete Bun.js course",
        }}
        data-aos="fade-up"
        data-aos-delay="200"
      />
      <CourseCard
        course={{
          duration: "2 weeks",
          image: {
            alt: "Course",
            src: "/courses/course-03.jpg",
          },
          numberOfModules: 20,
          title: "Complete CSS3 course",
        }}
        data-aos="fade-up"
        data-aos-delay="300"
      />

      <CourseCard
        course={{
          duration: "2 weeks",
          image: {
            alt: "Course",
            src: "/courses/course-04.jpg",
          },
          numberOfModules: 20,
          title: "Machine Learning A-Z: Hands-On Python and java",
        }}
        data-aos="fade-up"
        data-aos-delay="400"
      />
      <CourseCard
        course={{
          duration: "2 weeks",
          image: {
            alt: "Course",
            src: "/courses/course-05.jpg",
          },
          numberOfModules: 20,
          title: "Data Structure and Algorithms",
        }}
        data-aos="fade-up"
        data-aos-delay="500"
      />
      <CourseCard
        course={{
          duration: "2 weeks",
          image: {
            alt: "Course",
            src: "/courses/course-06.jpg",
          },
          numberOfModules: 20,
          title: "Rust crash course for beginners",
        }}
        data-aos="fade-up"
        data-aos-delay="600"
      />
    </div>

    <div data-aos="fade-up" data-aos-delay="700">
      <Button href="/courses" class="view-all-courses-btn">
        View All Courses
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="icon icon-tabler icon-tabler-arrow-narrow-right"
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
          <path d="M5 12l14 0m-4 4l4 -4m-4 -4l4 4" />
        </svg>
      </Button>
    </div>
  </div>
</section>

<style>
  .courses-section {
    padding: 8rem 0;
    overflow: hidden;
  }

  .courses-container {
    text-align: center;
    position: relative;
  }

  .courses-container::before,
  .courses-container::after,
  .courses-cards::before,
  .courses-cards::after {
    position: absolute;
  }

  .courses-container::before,
  .courses-cards::before {
    left: -15%;
  }

  .courses-container::after,
  .courses-cards::after {
    right: -15%;
  }

  .courses-container::before {
    top: 5%;
    content: url("/home/courses-decoration-1.png");
  }

  .courses-container::after {
    top: 10%;
    animation: top-bottom 4s linear infinite alternate;
    content: url("/home/courses-decoration-2.png");
  }

  .courses-cards::before {
    bottom: 10%;
    animation: top-bottom 4s linear infinite alternate;
    content: url("/home/courses-decoration-3.png");
  }

  .courses-cards::after {
    bottom: 5%;
    content: url("/home/courses-decoration-4.png");
  }

  .title > span {
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
    margin-bottom: 2.5rem;
  }

  .courses-cards {
    text-align: initial;
    grid-template-columns: 1fr 1fr 1fr;
    align-items: flex-start;
    gap: 1.875rem;
  }

  :global(.view-all-courses-btn) {
    margin-top: 3.75rem;
  }

  @media screen and (max-width: 57em) {
    .courses-cards {
      grid-template-columns: 1fr 1fr;
    }
  }

  @media screen and (max-width: 40em) {
    .courses-section {
      padding: 5rem 0;
    }

    .courses-container::before,
    .courses-container::after,
    .courses-cards::before,
    .courses-cards::after {
      display: none;
    }

    .courses-cards {
      grid-template-columns: 1fr;
    }
  }
</style>
