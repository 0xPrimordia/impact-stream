<script lang="ts">
    import Navbar from "../components/landing/Navbar.svelte";
    import Valueprop from "../components/landing/Valueprop.svelte";
    import Footer from "../components/landing/Footer.svelte";
    export let data;
</script>
<style>
    .wrapper section {
        max-width: 960px;
        margin: auto;
    }
</style>

<Navbar />
<div class="wrapper">
    <section>
        <h1>{data.hero.title}</h1>
        <p>{data.hero.sub}</p>
    </section>
</div>
<Valueprop />
<div class="wrapper">
    <section>
        <h1>Explainer Section</h1>
        <p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
    </section>
</div>
<div class="wrapper">
    <section>
        <h1>Team Section</h1>
        <p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
    </section>
</div>
<div class="wrapper">
    <section>
        <h1>Partners</h1>
        <p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
    </section>
</div>
<Footer />