<script lang="ts">
  import { page } from "$app/stores";
  import type { HTMLAnchorAttributes } from "svelte/elements";

  export let href: string;

  interface $$Props extends HTMLAnchorAttributes {}
</script>

<a
  class="nav-link"
  class:active={$page.url.pathname === href}
  {href}
  {...$$restProps}
  on:click
>
  <slot />
</a>

<style>
  .nav-link {
    padding: 1rem;
    text-decoration: none;
    display: inline-block;
    transition: color 0.2s ease;
    color: var(--clr-neutral-400);
    font-weight: var(--fw-600);
  }

  .nav-link.active,
  .nav-link:hover {
    color: var(--clr-accent-400);
  }

  .nav-link.active:hover {
    color: var(--clr-accent-600);
  }

  @media screen and (max-width: 40em) {
    .nav-link {
      width: 100%;
      padding: 0.5rem 2rem;
    }
  }
</style>
