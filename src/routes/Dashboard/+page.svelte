<script>
    import '$lib/global.css';
    import Navbar from '$lib/components/Navbar.svelte';
</script>

<Navbar />
<main>
    <h1>DASHBOARD</h1>
    <p>This is a simple Svelte page with global styles.</p>
</main>
<style>
    :global(*) {
        box-sizing: border-box;
    }

    main {
        padding: 1rem;
        margin: 0;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        min-height: 100vh;  /* Ensures the main element takes at least the full viewport height */
        width: 100%;        /* Ensures full width */
    }

    h1 {
        font-size: 2rem;
        color: var(--text);
        background-color: var(--secondary);
        border-radius: var(--border-radius-medium);
        padding: var(--spacing-small);
        text-align: center;
        max-width: 90%;    /* Prevents the h1 from overflowing its container */
        padding: 1rem;
    }

    p {
        font-size: 1rem;
        color: var(--text);
        margin-top: var(--spacing-small);
    }
</style>
