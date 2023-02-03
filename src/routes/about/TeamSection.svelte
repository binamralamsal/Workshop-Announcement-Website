<script lang="ts">
  const teams = [
    {
      name: "James Carlson",
      photo: "/about/person-01.jpg",
      position: "SEO Expert",
    },
    {
      name: "Nancy Phipps",
      photo: "/about/person-02.jpg",
      position: "UX Expert",
    },
    {
      name: "Troy Hall",
      photo: "/about/person-03.jpg",
      position: "Digital Marketer",
    },
    {
      name: "Isabelle Bruner",
      photo: "/about/person-04.jpg",
      position: "Next.js Expert",
    },
    {
      name: "Douglas Lage",
      photo: "/about/person-05.jpg",
      position: "Svelte Expert",
    },
    {
      name: "Linda Bacote",
      photo: "/about/person-06.jpg",
      position: "UX Expert",
    },
    {
      name: "John Moss",
      photo: "/about/person-07.jpg",
      position: "Digital Marketer",
    },
    {
      name: "Alice McCoy",
      photo: "/about/person-08.jpg",
      position: "Shitposter",
    },
  ];
</script>

<section class="team-section" aria-labelledby="events-title">
  <div class="container team-container">
    <header class="team-header">
      <h2 class="title" id="team-title">
        <span class="pre-title color-accent" data-aos="fade-up">
          Skilled Instructor
        </span>
        <span
          class="main-title color-heading"
          data-aos="fade-up"
          data-aos-delay="50"
        >
          Introduce our life Coaches
        </span>
      </h2>
    </header>

    <ul class="members">
      {#each teams as team, index}
        <li
          class="member"
          data-aos="fade-up"
          data-aos-delay={(index + 1) * 100}
        >
          <div class="photo">
            <div class="inner">
              <img src={team.photo} alt="" />

              <div class="socials">
                <a href="#" class="facebook">
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 320 512"
                    width="15"
                    height="15"
                    fill="currentColor"
                  >
                    <path
                      d="M279.14 288l14.22-92.66h-88.91v-60.13c0-25.35 12.42-50.06 52.24-50.06h40.42V6.26S260.43 0 225.36 0c-73.22 0-121.08 44.38-121.08 124.72v70.62H22.89V288h81.39v224h100.17V288z"
                    />
                  </svg>
                </a>
                <a href="#" class="linkedin">
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 448 512"
                    width="15"
                    height="15"
                    fill="currentColor"
                    ><path
                      d="M100.28 448H7.4V148.9h92.88zM53.79 108.1C24.09 108.1 0 83.5 0 53.8a53.79 53.79 0 0 1 107.58 0c0 29.7-24.1 54.3-53.79 54.3zM447.9 448h-92.68V302.4c0-34.7-.7-79.2-48.29-79.2-48.29 0-55.69 37.7-55.69 76.7V448h-92.78V148.9h89.08v40.8h1.3c12.4-23.5 42.69-48.3 87.88-48.3 94 0 111.28 61.9 111.28 142.3V448z"
                    />
                  </svg>
                </a>
                <a href="#" class="twitter">
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 512 512"
                    width="15"
                    height="15"
                    fill="currentColor"
                  >
                    <path
                      d="M459.37 151.716c.325 4.548.325 9.097.325 13.645 0 138.72-105.583 298.558-298.558 298.558-59.452 0-114.68-17.219-161.137-47.106 8.447.974 16.568 1.299 25.34 1.299 49.055 0 94.213-16.568 130.274-44.832-46.132-.975-84.792-31.188-98.112-72.772 6.498.974 12.995 1.624 19.818 1.624 9.421 0 18.843-1.3 27.614-3.573-48.081-9.747-84.143-51.98-84.143-102.985v-1.299c13.969 7.797 30.214 12.67 47.431 13.319-28.264-18.843-46.781-51.005-46.781-87.391 0-19.492 5.197-37.36 14.294-52.954 51.655 63.675 129.3 105.258 216.365 109.807-1.624-7.797-2.599-15.918-2.599-24.04 0-57.828 46.782-104.934 104.934-104.934 30.213 0 57.502 12.67 76.67 33.137 23.715-4.548 46.456-13.32 66.599-25.34-7.798 24.366-24.366 44.833-46.132 57.827 21.117-2.273 41.584-8.122 60.426-16.243-14.292 20.791-32.161 39.308-52.628 54.253z"
                    />
                  </svg>
                </a>
              </div>
            </div>
          </div>
          <h3 class="name color-heading">{team.name}</h3>
          <p class="position">{team.position}</p>
        </li>
      {/each}
    </ul>
  </div>
</section>

<style>
  .team-section {
    padding: 8rem 0;
    overflow: hidden;
    background: url("/home/blog-bg.jpg");
    background-repeat: no-repeat;
    background-size: cover;
  }

  .team-container {
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
    margin-bottom: 2rem;
  }

  .members {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    list-style-type: none;
    gap: 1.25rem;
  }

  .member {
    padding: 1.25rem;
  }

  .photo {
    padding: 1.25rem;
    margin-bottom: 1.6rem;
    position: relative;
  }

  .photo img {
    width: 100%;
  }

  .photo::before {
    content: "";
    left: 0;
    top: 0;
    bottom: 0;
    right: 0;
    position: absolute;
    background-image: url("/about/photo-outer.png");
    aspect-ratio: 1/1;
    background-size: contain;
    transition: all 0.5s;
  }

  .inner {
    position: relative;
  }

  .inner::before {
    content: "";
    background: var(--clr-accent-900);
    opacity: 0;
    top: 0;
    bottom: 0;
    right: 0;
    left: 0;
    position: absolute;
    border-radius: 100%;
    transition: all 0.5s;
  }

  .member:hover .photo::before {
    transform: rotate(90deg);
  }

  .member:hover .inner::before {
    opacity: 0.4;
  }

  .position {
    transition: 0.5s all;
  }

  .member:hover .position {
    color: var(--clr-accent-400);
  }

  .photo img {
    border-radius: 100%;
  }

  .socials {
    position: absolute;
    top: 50%;
    left: 50%;
    display: flex;
    gap: 0.25rem;
    transform: translate(-50%, -50%);
  }

  .socials a {
    padding: 0.5rem;
    background: white;
    display: flex;
    border-radius: 100%;
    opacity: 0;
    visibility: hidden;
    transform: translateY(0.5rem);
    transition: all 0.45s cubic-bezier(0.23, 0.88, 0.34, 0.99);
  }

  .member:hover .socials a {
    transform: translateY(0);
    opacity: 1;
    visibility: visible;
  }

  .member .facebook {
    transition-delay: 0.07692s;
  }

  .member .linkedin {
    transition-delay: 0.15385s;
  }

  .member .twitter {
    transition-delay: 0.23077s;
  }

  .name {
    font-size: var(--fs-500);
    font-weight: var(--fw-700);
    margin-bottom: 0.3125rem;
  }

  @media screen and (max-width: 58em) {
    .members {
      grid-template-columns: repeat(3, 1fr);
    }
  }

  @media screen and (max-width: 48em) {
    .team-section {
      padding: 5rem 0;
    }

    .main-title {
      margin-bottom: 2rem;
    }

    .members {
      grid-template-columns: repeat(2, 1fr);
    }
  }

  @media screen and (max-width: 32em) {
    .members {
      grid-template-columns: 1fr;
    }
  }
</style>
