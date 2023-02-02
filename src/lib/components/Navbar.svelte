<script lang="ts">
  import { page } from "$app/stores";
  import NavLink from "./NavLink.svelte";

  let navbarOpened = false;
  let scrolled = false;

  const handleOnScroll = () => {
    if (window.scrollY > 100) {
      return (scrolled = true);
    }

    return (scrolled = false);
  };

  const handleToggleNavbar = () => (navbarOpened = !navbarOpened);

  const pagesWithTransparentNavbar = ["/"];
</script>

<svelte:window on:scroll={handleOnScroll} />

<header
  class="navbar-wrapper"
  class:transparent={pagesWithTransparentNavbar.includes($page.url.pathname)}
  class:scrolled
>
  <div class="container nav-container">
    <a data-aos="fade-right" href="/">Event</a>

    <button
      aria-controls="primary-navigation"
      aria-expanded={navbarOpened}
      aria-label="toggle navigation"
      class="mobile-nav-toggle"
      class:active={navbarOpened}
      on:click={handleToggleNavbar}
    >
      <span />
      <span />
      <span />
    </button>

    <nav
      class="primary-navigation"
      class:active={navbarOpened}
      data-aos="fade-left"
      data-aos-delay="250"
      id="primary-navigation"
    >
      <ul class="nav-links">
        <li>
          <NavLink href="/" on:click={handleToggleNavbar}>Home</NavLink>
        </li>
        <li>
          <NavLink href="/about" on:click={handleToggleNavbar}>About</NavLink>
        </li>
        <li>
          <NavLink href="/course-details" on:click={handleToggleNavbar}
            >Course Details</NavLink
          >
        </li>
        <li>
          <NavLink
            href="https://forms.google.com"
            target="_blank"
            on:click={handleToggleNavbar}
          >
            Register
          </NavLink>
        </li>
      </ul>
    </nav>
  </div>
</header>

<style>
  .navbar-wrapper {
    padding: 1rem 0;
    position: relative;
    top: 0;
    z-index: 999;
  }

  .navbar-wrapper.transparent {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
  }

  .navbar-wrapper.scrolled {
    padding: 0.5rem 0;
    position: sticky;
    background-color: white;
    animation: headerSticky 0.95s ease forwards;
  }

  .navbar-wrapper.transparent.scrolled {
    position: fixed;
  }

  @keyframes headerSticky {
    from {
      transform: translateY(-100%);
    }
    to {
      transform: translateY(0);
    }
  }

  .nav-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .nav-links {
    list-style-type: none;
    display: flex;
    gap: 0.5rem;
  }

  .mobile-nav-toggle {
    display: none;
    background: none;
    border: 0;
    flex-direction: column;
    padding: 0.5rem;
    cursor: pointer;
    gap: 0.3rem;
  }

  .mobile-nav-toggle span {
    background: var(--clr-neutral-400);
    display: inline-block;
    padding: 0.05rem 0.55rem;
    transition: all 0.2s ease 0s;
    transform-origin: left center;
  }

  .mobile-nav-toggle.active span:first-child {
    transform: rotate(45deg);
  }

  .mobile-nav-toggle.active span:nth-child(2) {
    opacity: 0;
  }

  .mobile-nav-toggle.active span:last-child {
    transform: rotate(-45deg);
  }

  @media screen and (max-width: 40em) {
    .navbar-wrapper {
      padding: 0.5rem 0;
    }

    .primary-navigation {
      display: none;
      position: absolute;
      top: 100%;
      height: 0;
      background: white;
      left: 0;
      animation: height 0.2s ease;
      right: 0;
    }

    .primary-navigation.active {
      display: block;
      height: auto;
    }

    .nav-links {
      flex-direction: column;
      gap: 0;
    }

    .mobile-nav-toggle {
      display: flex;
    }
  }
</style>
