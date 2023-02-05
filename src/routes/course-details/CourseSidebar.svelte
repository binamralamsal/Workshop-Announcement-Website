<script lang="ts">
  import Button from "$lib/components/Button.svelte";
</script>

<aside class="course-sidebar">
  <ul>
    <li>
      <span class="stat-title">
        <span class="icon">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="icon-tabler icon-tabler-clock"
            width="14"
            height="14"
            viewBox="0 0 24 24"
            stroke-width="2"
            stroke="currentColor"
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
            <path d="M12 12m-9 0a9 9 0 1 0 18 0a9 9 0 1 0 -18 0" />
            <path d="M12 7l0 5l3 3" />
          </svg>
        </span>
        Duration
      </span>
      <span>3 days</span>
    </li>

    <li>
      <span class="stat-title">
        <span class="icon">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="icon icon-tabler icon-tabler-chart-bar"
            width="14"
            height="14"
            viewBox="0 0 24 24"
            stroke-width="2"
            stroke="currentColor"
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
            <path
              d="M3 12m0 1a1 1 0 0 1 1 -1h4a1 1 0 0 1 1 1v6a1 1 0 0 1 -1 1h-4a1 1 0 0 1 -1 -1z"
            />
            <path
              d="M9 8m0 1a1 1 0 0 1 1 -1h4a1 1 0 0 1 1 1v10a1 1 0 0 1 -1 1h-4a1 1 0 0 1 -1 -1z"
            />
            <path
              d="M15 4m0 1a1 1 0 0 1 1 -1h4a1 1 0 0 1 1 1v14a1 1 0 0 1 -1 1h-4a1 1 0 0 1 -1 -1z"
            />
            <path d="M4 20l14 0" />
          </svg>
        </span>
        Skill Level
      </span>
      <span>Advanced</span>
    </li>

    <li>
      <span class="stat-title">
        <span class="icon">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="icon icon-tabler icon-tabler-world"
            width="14"
            height="14"
            viewBox="0 0 24 24"
            stroke-width="2"
            stroke="currentColor"
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
            <path d="M12 12m-9 0a9 9 0 1 0 18 0a9 9 0 1 0 -18 0" />
            <path d="M3.6 9l16.8 0" />
            <path d="M3.6 15l16.8 0" />
            <path d="M11.5 3a17 17 0 0 0 0 18" />
            <path d="M12.5 3a17 17 0 0 1 0 18" />
          </svg>
        </span>
        Language
      </span>
      <span>English</span>
    </li>

    <li>
      <span class="stat-title">
        <span class="icon">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="icon icon-tabler icon-tabler-certificate"
            width="14"
            height="14"
            viewBox="0 0 24 24"
            stroke-width="2"
            stroke="currentColor"
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
            <path d="M15 15m-3 0a3 3 0 1 0 6 0a3 3 0 1 0 -6 0" />
            <path d="M13 17.5v4.5l2 -1.5l2 1.5v-4.5" />
            <path
              d="M10 19h-5a2 2 0 0 1 -2 -2v-10c0 -1.1 .9 -2 2 -2h14a2 2 0 0 1 2 2v10a2 2 0 0 1 -1 1.73"
            />
            <path d="M6 9l12 0" />
            <path d="M6 12l3 0" />
            <path d="M6 15l2 0" />
          </svg>
        </span>
        Certificate
      </span>
      <span>Yes</span>
    </li>

    <li>
      <span class="stat-title">
        <span class="icon">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="icon icon-tabler icon-tabler-calendar"
            width="14"
            height="14"
            viewBox="0 0 24 24"
            stroke-width="2"
            stroke="currentColor"
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
            <path
              d="M4 5m0 2a2 2 0 0 1 2 -2h12a2 2 0 0 1 2 2v12a2 2 0 0 1 -2 2h-12a2 2 0 0 1 -2 -2z"
            />
            <path d="M16 3l0 4" />
            <path d="M8 3l0 4" />
            <path d="M4 11l16 0" />
            <path d="M11 15l1 0" />
            <path d="M12 15l0 3" />
          </svg>
        </span>
        Deadline
      </span>
      <span>20th Feb, 2023</span>
    </li>

    <li>
      <span class="stat-title">
        <span class="icon">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="icon icon-tabler icon-tabler-user"
            width="14"
            height="14"
            viewBox="0 0 24 24"
            stroke-width="2"
            stroke="currentColor"
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
            <path d="M12 7m-4 0a4 4 0 1 0 8 0a4 4 0 1 0 -8 0" />
            <path d="M6 21v-2a4 4 0 0 1 4 -4h4a4 4 0 0 1 4 4v2" />
          </svg>
        </span>
        Instructor
      </span>
      <span>Nancy Philipps</span>
    </li>

    <li class="last-detail">
      <span class="stat-title">
        <span class="icon">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="icon icon-tabler icon-tabler-currency-rupee-nepalese"
            width="14"
            height="14"
            viewBox="0 0 24 24"
            stroke-width="2"
            stroke="currentColor"
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
          >
            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
            <path d="M15 5h-11h3a4 4 0 1 1 0 8h-3l6 6" />
            <path d="M21 17l-4.586 -4.414a2 2 0 0 0 -2.828 2.828l.707 .707" />
          </svg>
        </span>
        Price
      </span>
      <span>Rs. 500</span>
    </li>
  </ul>
  <Button size="large" href="https://forms.google.com">
    Register
    <svg
      class="icon-tabler icon-tabler-arrow-right s-xcnQQNRdRv-M"
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
      <path
        d="M0 0h24v24H0z"
        fill="none"
        stroke="none"
        class="s-xcnQQNRdRv-M"
      />
      <line x1="5" x2="19" y1="12" y2="12" class="s-xcnQQNRdRv-M" /><line
        x1="13"
        x2="19"
        y1="18"
        y2="12"
        class="s-xcnQQNRdRv-M"
      />
      <line x1="13" x2="19" y1="6" y2="12" class="s-xcnQQNRdRv-M" />
    </svg>
  </Button>
</aside>

<style>
  .course-sidebar {
    background: white;
    border-radius: var(--radius-600);
    box-shadow: 0 10px 30px rgb(0 0 0 / 7%);
    align-self: flex-start;
    padding: 2.5rem;
    position: sticky;
    top: 5rem;
    display: flex;
    gap: 1rem;
    flex-direction: column;
  }

  ul {
    list-style-type: none;
  }

  li {
    display: flex;
    justify-content: space-between;
    padding: 1rem 0;
    flex-wrap: wrap;
    border-bottom: 1px solid #eee;
  }

  .icon {
    color: var(--clr-accent-400);
  }

  .last-detail {
    border-bottom: 0;
  }

  li > span {
    display: flex;
    align-items: center;
    gap: 1rem;
  }

  .stat-title {
    font-weight: var(--fw-600);
  }

  @media screen and (max-width: 57em) {
    .course-sidebar {
      padding: 1rem 1.5rem 1rem 1.5rem;
    }
  }
</style>
