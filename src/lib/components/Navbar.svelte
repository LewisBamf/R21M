<script>
    import { goto } from '$app/navigation'; // Import the goto function for navigation
    import logo from '../../assets/logo.svg';

    let isMenuOpen = false;

    function toggleMenu() {
        isMenuOpen = !isMenuOpen;
    }

    // @ts-ignore
    function navigateTo(url) {
        goto(url); // Use SvelteKit's goto function for navigation
        if (window.innerWidth <= 853) {
            toggleMenu(); // Close the menu after navigation only on mobile
        }
    }
</script>

<style>
    /* Your existing styles */
    .navbar {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 0.6rem;
        background-color: var(--secondary);
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        z-index: 1000;
        color: var(--text);
        margin-bottom: 2rem;
    }

    .logo {
        width: 50px;
        height: auto;
        cursor: pointer;
    }

    .pages {
        display: flex;
        gap: 5rem;
        margin-right: calc(50% - 10rem);
    }

    .page {
        position: relative;
        cursor: pointer;
        color: var(--text);
        background-color: rgba(0, 0, 0, 0);
        border: none;
    }

    .page:hover {
        color: var(--secondary);
    }

    .page::after {
        content: "";
        position: absolute;
        bottom: -2px;
        left: 0;
        width: 100%;
        height: 2px;
        background-color: var(--secondary);
        transform: scaleX(0);
        transition: transform 0.3s;
    }

    .page:hover::after {
        transform: scaleX(1);
    }

    .hamburger {
        cursor: pointer;
        display: none;
        margin-right: 2rem;
        background-color: rgba(0, 0, 0, 0);
        border: none;
    }

    .hamburger input {
        display: none;
    }

    .hamburger svg {
        height: 3em;
        transition: transform 400ms cubic-bezier(0.4, 0, 0.2, 1);
    }

    .line {
        fill: none;
        stroke: white;
        stroke-linecap: round;
        stroke-linejoin: round;
        stroke-width: 3;
        transition: stroke-dasharray 400ms cubic-bezier(0.4, 0, 0.2, 1),
                    stroke-dashoffset 400ms cubic-bezier(0.4, 0, 0.2, 1);
    }

    .line-top-bottom {
        stroke-dasharray: 12 63;
    }

    .hamburger input:checked + svg {
        transform: rotate(-45deg);
    }

    .hamburger input:checked + svg .line-top-bottom {
        stroke-dasharray: 20 300;
        stroke-dashoffset: -32.42;
    }

    .menu {
        position: absolute;
        top: 100%;
        right: -100%;
        width: 100%;
        padding: 1rem;
        background-color: var(--secondary);
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.3);
        transition: right 0.4s ease-in-out;
        align-content: center;
        justify-content: center;
        
    }

    .menu.open {
        right: 0%;
        text-align: center;
    }

    .menu .page {
        display: block;
        padding: 0.5rem 0.5rem;
        color: var(--text);
        align-content: center;
        justify-content: center;
        text-align: center;
        text-align: center;
        font-size: 2rem;
    }

    @media (max-width: 853px) {
        .pages {
            display: none;
        }

        .hamburger {
            display: flex;
        }
    }
</style>

<div class="navbar">
    <!-- svelte-ignore a11y-no-noninteractive-element-interactions -->
    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <img src={logo} alt="Logo" class="logo" on:click={() => navigateTo('/')} on:keydown={(e) => {if (e.key === 'Enter') navigateTo('/')}}>
    <div class="pages">
        <button on:click={() => navigateTo('/')} on:keydown={(e) => {if (e.key === 'Enter') navigateTo('/')}} class="page" type="button" aria-label="Home">Home</button>
        <button on:click={() => navigateTo('/Login')} class="page" aria-label="Login">Login</button>
        <button on:click={() => navigateTo('/Dashboard')} class="page" aria-label="Dashboard">Dashboard</button>
    </div>
    <button class="hamburger" on:click={toggleMenu}>
        <input type="checkbox" bind:checked={isMenuOpen}>
        <svg viewBox="0 0 32 32">
            <path class="line line-top-bottom" d="M27 10 13 10C10.8 10 9 8.2 9 6 9 3.5 10.8 2 13 2 15.2 2 17 3.8 17 6L17 26C17 28.2 18.8 30 21 30 23.2 30 25 28.2 25 26 25 23.8 23.2 22 21 22L7 22"></path>
            <path class="line" d="M7 16 27 16"></path>
        </svg>
    </button>
    <div class="menu {isMenuOpen ? 'open' : ''}">
        <button on:click={() => navigateTo('/')} on:keydown={(e) => {if (e.key === 'Enter') navigateTo('/')}} class="page" type="button" aria-label="Home">Home</button>
        <button on:click={() => navigateTo('/Login')} class="page" aria-label="Login">Login</button>
        <button on:click={() => navigateTo('/Dashboard')} class="page" aria-label="Dashboard">Dashboard</button>
    </div>
</div>