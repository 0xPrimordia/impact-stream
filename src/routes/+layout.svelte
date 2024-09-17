<script>
  import { setContext } from 'svelte';
  import { page } from '$app/stores';
</script>

<svelte:head>
  {#if $page.url.pathname === '/'}
    <title>Impact Stream | Digital → IRL Impact</title>
    <meta name="description" content="We are decentralizing poverty alleviation and creating transparent streams of impact to developing communities." />
    <meta property="og:title" content="Impact Stream | Digital → IRL Impact" />
    <meta property="og:description" content="We are decentralizing poverty alleviation and creating transparent streams of impact to developing communities." />
    <meta property="og:image" content="https://impact.stream/images/og-image-2.png" />
  {/if}
</svelte:head>

<slot />