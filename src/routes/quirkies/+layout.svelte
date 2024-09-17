<script>
  import { setContext } from 'svelte';
  import { page } from '$app/stores';
</script>

<svelte:head>
  {#if $page.url.pathname.startsWith('/quirkies')}
    <title>Togo Water Campaign with Quirkies</title>
    <meta name="description" content="Impact Stream is partnering with Quirkies to build wells and bring clean water to both a village and an orphanage in Togo, West Africa." />
    <meta property="og:title" content="Togo Water Campaign with Quirkies" />
    <meta property="og:description" content="Impact Stream is partnering with Quirkies to build wells and bring clean water to both a village and an orphanage in Togo, West Africa." />
    <meta property="og:image" content="https://impact.stream/images/quirkies-og-image.png" />
  {/if}
</svelte:head>

<slot />