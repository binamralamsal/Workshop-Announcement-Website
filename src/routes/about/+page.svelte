<script lang="ts">
  import { PageHeader } from "$lib/components";
  import AboutSection from "./AboutSection.svelte";
  import AwardSection from "./AwardSection.svelte";
  import OfferSection from "./OfferSection.svelte";
  import TeamSection from "./TeamSection.svelte";
  import UpcomingEventSection from "./UpcomingEventSection.svelte";
  import WorkshopSection from "./WorkshopSection.svelte";
</script>

<svelte:head>
  <title>About | Xavier Entrepreneurship Bootcamp</title>
</svelte:head>

<PageHeader title="About Us" />
<AboutSection />
<OfferSection />
<WorkshopSection />
<TeamSection />
<UpcomingEventSection />
<AwardSection />
