<script>
    import '$lib/global.css';
    import Navbar from '$lib/components/Navbar.svelte';
</script>

<Navbar />
<main>
    <h1>Financial Dashboard</h1>
    <section class="stats-overview">
        <div class="stat-box">
            <h2>Total Savings</h2>
            <p>$250,000</p>
        </div>
        <div class="stat-box">
            <h2>Monthly Contributions</h2>
            <p>$5,000</p>
        </div>
        <div class="stat-box">
            <h2>Goal</h2>
            <p>$1,000,000</p>
        </div>
    </section>

    <section class="progress-tracker">
        <h2>Progress to $1 Million</h2>
        <div class="progress-bar-container">
            <div class="progress-bar" style="width: 25%;"></div>
        </div>
    </section>

    <section class="recent-activity">
        <h2>Recent Activity</h2>
        <ul>
            <li>Deposited $1,000 on 20th Aug 2024</li>
            <li>Invested $2,000 in Stocks on 15th Aug 2024</li>
            <li>Received $500 in Dividends on 10th Aug 2024</li>
        </ul>
    </section>

    <section class="upcoming-tasks">
        <h2>Upcoming Financial Tasks</h2>
        <ul>
            <li>Review Investment Portfolio</li>
            <li>Plan Next Month's Contributions</li>
            <li>Analyze Market Trends</li>
        </ul>
    </section>
</main>

<style>
    :global(*) {
        box-sizing: border-box;
    }

    main {
        padding: 2rem;
        margin: 0;
        display: flex;
        flex-direction: column;
        justify-content: flex-start;
        align-items: center;
        min-height: 100vh;
        width: 100%;
        background-color: var(--primary);
    }

    h1 {
        font-size: 2.5rem;
        color: var(--text);
        background-color: var(--secondary);
        border-radius: var(--border-m);
        padding: var(--spacing-m);
        text-align: center;
        width: 100%;
        max-width: 800px;
        margin-bottom: 2rem;
    }

    .stats-overview {
        display: flex;
        justify-content: space-around;
        width: 100%;
        max-width: 800px;
        margin-bottom: 2rem;
    }

    .stat-box {
        background-color: var(--secondary);
        padding: var(--spacing-s);
        border-radius: var(--border-m);
        text-align: center;
        flex: 1;
        margin: 0 1rem;
    }

    .stat-box h2 {
        font-size: 1.25rem;
        color: var(--text);
    }

    .stat-box p {
        font-size: 1.5rem;
        color: var(--text);
    }

    .progress-tracker {
        width: 100%;
        max-width: 800px;
        margin-bottom: 2rem;
    }

    .progress-tracker h2 {
        font-size: 1.5rem;
        color: var(--text);
        margin-bottom: 1rem;
    }

    .progress-bar-container {
        width: 100%;
        background-color: var(--secondary);
        border-radius: var(--border-s);
        overflow: hidden;
    }

    .progress-bar {
        height: 1.5rem;
        background-color: var(--primary);
    }

    .recent-activity,
    .upcoming-tasks {
        width: 100%;
        max-width: 800px;
        margin-bottom: 2rem;
    }

    .recent-activity h2,
    .upcoming-tasks h2 {
        font-size: 1.5rem;
        color: var(--text);
        margin-bottom: 1rem;
    }

    ul {
        list-style-type: none;
        padding: 0;
    }

    li {
        background-color: var(--secondary);
        color: var(--text);
        padding: var(--spacing-small);
        border-radius: var(--border-s);
        margin-bottom: var(--spacing-s);
    }
</style>
