<script lang="ts">
  export let title: string;
  type BreadCrumbItem = {
    title: string;
    href: string;
  };

  export let breadcrumbs: BreadCrumbItem[] = [];
</script>

<section class="header">
  <div class="container container">
    <h1 class="page-title color-heading" data-aos="fade-up">{title}</h1>
    <nav class="breadcrumb" data-aos="fade-right" data-aos-delay="100">
      <ul>
        <li>
          <a href="/">Home</a>
        </li>
        <li class="separator">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="icon icon-tabler icon-tabler-chevron-right"
            width="16"
            height="16"
            viewBox="0 0 24 24"
            stroke-width="2"
            stroke="currentColor"
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
            <path d="M9 6l6 6l-6 6" />
          </svg>
        </li>

        {#each breadcrumbs as }
          
        {/each}

        <li>{title}</li>
      </ul>
    </nav>
  </div>
</section>

<style>
  .header {
    padding: 3.75rem 0;
    background: url("/header-bg.jpg");
    overflow: hidden;
  }

  .page-title {
    margin-bottom: 0.3125rem;
    font-size: var(--fs-700);
    font-weight: var(--fw-800);
    line-height: 1.4;
    position: relative;
  }

  .container {
    position: relative;
  }

  .container::before,
  .container::after,
  .page-title::before,
  .page-title::after,
  .breadcrumb::before,
  .breadcrumb::after {
    position: absolute;
  }

  .container::before {
    content: url("/courses/course-decoration-1.png");
    left: -20%;
    top: -40%;
  }

  .container::after {
    content: url("/courses/course-decoration-6.png");
    right: -25%;
    bottom: -40%;
  }

  .page-title::before {
    content: url("/courses/course-decoration-2.png");
    left: -10%;
    bottom: -130%;
  }

  .page-title::after {
    content: url("/courses/course-decoration-3.png");
    left: 30%;
    bottom: -130%;
  }

  .breadcrumb::before {
    content: url("/courses/course-decoration-4.png");
    left: 60%;
    top: -20%;
  }

  .breadcrumb::after {
    content: url("/courses/course-decoration-5.png");
    right: -10%;
    top: -20%;
  }

  ul {
    list-style-type: none;
    display: flex;
    align-items: center;
    gap: 0.75rem;
  }

  ul,
  a {
    color: var(--clr-neutral-400);
  }

  a:hover {
    color: var(--clr-accent-400);
  }

  ul li {
    display: flex;
  }

  @media screen and (max-width: 48em) {
    .header {
      padding: 2rem 0;
    }

    .container::before,
    .container::after,
    .page-title::before,
    .page-title::after,
    .breadcrumb::before,
    .breadcrumb::after {
      display: none;
    }
  }
</style>
