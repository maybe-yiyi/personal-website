<script>
    import { NavBar } from '$lib';
</script>

<div id="main">
    <NavBar />
    <section id="hero">
        <div id="hero-content">
            <p id="hello">Hello I'm</p>
            <h1>Yiyoung<br />Liu</h1>
            <p>Information Systems @ CMU<br />Class of 2029</p>
        </div>
    </section>
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

    /* hero stuff */
    #hero {
        min-height: 100vh;
        display: flex;
        align-items: center;
        padding: 20px 8px;
    }

    #hero-content {
        max-width: 48rem;
        width: 100%;
        margin-inline: auto;
    }

    #hello {
        font-size: 0.75rem;
        text-transform: uppercase;
        color: #01A4FF;
        margin-botton: 1.5rem;
    }

    #hero-content h1 {
        font-family: sans-serif;
        font-size: 8rem;
        font-weight: bold;

        margin-top: 0rem;
        margin-bottom: 1.5rem;
    }
</style>
