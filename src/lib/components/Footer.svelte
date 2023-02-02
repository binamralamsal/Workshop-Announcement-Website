<script>
  import Arrow from "$lib/assets/icons/Arrow.svelte";
</script>

<footer>
  <p class="copyright-text">
    Copyright {new Date().getFullYear()}. Made by Xavier Computer and Coding
    Club
  </p>
</footer>

<style>
  footer {
    background: var(--clr-accent-900);
    overflow: hidden;
    color: white;
  }

  .copyright-text {
    text-align: center;
    padding: 2rem;
  }
</style>
