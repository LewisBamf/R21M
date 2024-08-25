<script>
    import '$lib/global.css';
    import Navbar from '$lib/components/Navbar.svelte';
</script>

<Navbar />
<main>
    <h1>LOGIN</h1>
    <form>
        <div class="input-group">
            <label for="username">Username</label>
            <input type="text" id="username" name="username" required>
        </div>
        <div class="input-group">
            <label for="password">Password</label>
            <input type="password" id="password" name="password" required>
        </div>
        <button type="submit">Login</button>
    </form>
</main>

<style>
    main {
        padding: 1rem;
        margin: 0;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        min-height: 100vh;
        width: 100%;
    }

    h1 {
        font-size: 2rem;
        color: var(--text);
        background-color: var(--secondary);
        border-radius: var(--border-m);
        padding: var(--spacing-m);
        text-align: center;
        max-width: 90%;
    }

    form {
        display: flex;
        flex-direction: column;
        gap: var(--spacing-m);
        width: 100%;
        max-width: 300px;
    }

    .input-group {
        display: flex;
        flex-direction: column;
    }

    label {
        font-size: 1rem;
        color: var(--text);
        margin-bottom: var(--spacing-s);
    }

    input {
        padding: var(--spacing-s);
        font-size: 1rem;
        border-radius: var(--border-s);
        border: 1px solid var(--tertiary);
        background-color: var(--dark);
        color: var(--text);
    }

    button {
        padding: var(--spacing-m);
        font-size: 2rem;
        color: var(--text);
        background-color: var(--secondary);
        border: none;
        border-radius: var(--border-m);
        cursor: pointer;
        transition: background-color 0.3s;
    }

    button:hover {
        background-color: var(--accent);
    }
</style>
