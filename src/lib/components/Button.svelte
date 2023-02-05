<script lang="ts">
  import type { HTMLButtonAttributes } from "svelte/elements";

  type Variant = "primary" | "dark-primary" | "light-secondary";
  type Size = "default" | "large";

  export let href: string | undefined = undefined;
  export let variant: Variant = "primary";
  export let size: Size = "default";

  interface $$Props extends HTMLButtonAttributes {
    href?: string | undefined;
    variant?: Variant;
    size?: Size;
  }
</script>

<svelte:element
  this={href ? "a" : "button"}
  {...$$restProps}
  class:btn={true}
  class:primary={variant === "primary"}
  class:dark-primary={variant === "dark-primary"}
  class:light-secondary={variant === "light-secondary"}
  class:large={size === "large"}
  {href}
>
  <slot />
</svelte:element>

<style>
  .btn {
    background: none;
    border: none;
    text-decoration: none;
    padding: 0.75em 1.875em;
    color: var(--clr-neutral-400);
    border-radius: var(--radius-400);
    transition: all 0.2s ease;
    cursor: pointer;
    font-weight: var(--fw-700);

    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: 0.5rem;
  }

  .large {
    padding: 1em 2em;
  }

  .primary,
  .dark-primary:hover {
    background: var(--clr-accent-400);
    color: var(--clr-neutral-100);
  }

  .primary:hover,
  .dark-primary {
    color: var(--clr-neutral-100);
    background: var(--clr-accent-600);
  }

  .light-secondary {
    color: var(--clr-accent-400);
    background: white;
  }

  .light-secondary:hover {
    color: white;
    background: var(--clr-secondary-400);
  }
</style>
