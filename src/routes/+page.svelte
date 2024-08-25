<script>
    import '$lib/global.css';
    import Navbar from '$lib/components/Navbar.svelte';
</script>

<Navbar />
<main>
    <section class="hero">
        <h1>Road to 1 Million</h1>
        <p>Your journey to financial independence starts here.</p>
        <button class="cta-button">Get Started</button>
    </section>

    <section class="features">
        <div class="feature">
            <h2>Track Your Progress</h2>
            <p>See how close you are to reaching your goal with our intuitive tracking tools.</p>
        </div>
        <div class="feature">
            <h2>Smart Saving Tips</h2>
            <p>Get personalized tips to maximize your savings and accelerate your journey.</p>
        </div>
        <div class="feature">
            <h2>Community Support</h2>
            <p>Join a community of like-minded savers and share your progress.</p>
        </div>
    </section>
</main>

<style>
    :global(*) {
        box-sizing: border-box;
    }

    main {
        display: flex;
        flex-direction: column;
        justify-content: top;
        align-items: top;
        min-height: 100vh;
        padding: 1rem;
        background-color: var(--primary);
        color: var(--text);
    }

    .hero {
        text-align: center;
        margin-bottom: 2rem;
        background: var(--secondary);
        padding: 2rem;
        margin-top: 5rem;
        border-radius: var(--border-l);
        box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        transition: transform 0.3s ease;
    }

    .hero:hover {
        transform: translateY(-5px);
    }

    h1 {
        font-size: 2.5rem;
        color: var(--text-light);
        margin-bottom: 1rem;
    }

    p {
        font-size: 1.2rem;
        color: var(--text-light);
        margin-top: var(--spacing-s);
    }

    .cta-button {
        background-color: var(--tertiary);
        color: white;
        padding: var(--spacing-m) var(--spacing-l);
        border: none;
        border-radius: var(--border-m);
        cursor: pointer;
        font-size: 1rem;
        margin-top: var(--spacing-m);
        transition: background-color 0.3s ease, transform 0.3s ease;
    }

    .cta-button:hover {
        background-color: var(--secondary);
        transform: translateY(-3px);
    }

    .features {
        display: flex;
        justify-content: space-around;
        flex-wrap: wrap;
        width: 100%;
        max-width: 1200px;
        gap: 2rem;
    }

    .feature {
        background-color: var(--dark);
        color: var(--text-light);
        padding: var(--spacing-m);
        border-radius: var(--border-xl);
        flex: 1;
        min-width: 250px;
        max-width: 300px;
        text-align: center;
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .feature:hover {
        transform: translateY(-5px);
        box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
    }

    .feature h2 {
        font-size: 1.5rem;
        margin-bottom: var(--spacing-s);
    }

    .feature p {
        font-size: 1rem;
        margin-top: 0;
    }
</style>
