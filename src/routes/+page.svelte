<script>
    import { NavBar, Hero } from '$lib';
</script>

<div id="main">
    <NavBar />
    <Hero />
</div>

<style>
    :global(body) {
        margin: 0;
        padding: 0;

        background-color: black;
        font-family: 'Geist Mono', monospace;
        scrollbar-width: none;
    }

    :global(body::-webkit-scrollbar),
    :global(html::-webkit-scrollbar) {
        display: none;
    }

    #main {
        color: white;
    }
</style>
