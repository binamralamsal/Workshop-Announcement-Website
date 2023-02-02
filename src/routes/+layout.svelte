<script lang="ts">
  import NProgress from "nprogress";
  import { navigating } from "$app/stores";
  import Aos from "aos";

  import { Navbar, Footer } from "$lib/components";

  import "nprogress/nprogress.css";
  import "$lib/styles/css-reset.css";
  import "$lib/styles/styles.css";
  import "aos/dist/aos.css";

  import { onMount } from "svelte";

  onMount(() => {
    Aos.init({ once: true, duration: 750 });
  });

  NProgress.configure({
    minimum: 0.16,
  });

  $: {
    if ($navigating) {
      NProgress.start();
    }
    if (!$navigating) {
      NProgress.done();
    }
  }
</script>

<Navbar /><slot />
<Footer />
