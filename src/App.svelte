<!-- <script>
	export let name;
</script>

<main>
	<h1>Hello {name}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style> -->

<script>
/*
    // JavaScript logic for the component would go here
    import { onMount, onDestroy, tick } from 'svelte';
    import tsParticles from 'tsparticles';

    let posts = [];
    const MAX_POSTS = 50;
    let intervalId;

    // Function to fetch data from the API
    async function fetchPosts() {
        try {
            const response = await fetch('https://jsonplaceholder.typicode.com/posts');
            const data = await response.json();
        
            // Append new posts to the array
            posts = [...data, ...posts];

            // Limit the posts array to the most recent 50 posts
            if (posts.length > MAX_POSTS) {
                posts = posts.slice(0, MAX_POSTS);
            }
        } catch (error) {
            console.error('Error fetching data:', error);
        }
    }

    // Fetch data on component mount and set up the interval
    onMount(() => {
        // Fetch posts initially
        fetchPosts();

        // Set up interval to fetch posts every 3 minutes
        intervalId = setInterval(async () => {
            await fetchPosts();
            await tick();  // Ensure DOM is updated after fetching data
        }, 180000); // 180,000 ms = 3 minutes

        // Initialize the particles effect in the background
        tsParticles.load('particles-js',{
            selector: '#particles-js',  // The container where the particles will appear
            color: {
                value: '#ffffff',
            },
            particles: {
                number: {
                value: 50,
                },
                shape: {
                type: 'circle',
                },
                opacity: {
                value: 0.5,
                },
                size: {
                value: 3,
                },
                move: {
                speed: 1,
                },
            },
        });

    });
    
    // Clean up interval when the component is destroyed
    onDestroy(() => {
        clearInterval(intervalId);
    });

*/
</script>

<style>
    /* Global style */
    :global(body) {
        margin: 0;
        font-family: 'Arial', sans-serif;
        background-color: #2c2c2c; /* Dark background */
        color: #e0e0e0; /* Light text color */
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: flex-start;
        height: 100vh;
    }

    /* Container for particles background */
    #particles-js {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        z-index: -1; /* Put particles behind content */
    }
	/* Main container style */
	main {
        display: flex;
        flex-direction: column;
        align-items: center; /* Center items horizontally */
        text-align: center; /* Center text */
    }

    /* Header style */
    header {
        text-align: center;
        margin-top: 20px;
        font-size: 3em;
        color: #ffc107; /* Gold-like color to match medieval tones */
        font-weight: bold;
        text-shadow: 2px 2px 0px #6c757d, -2px -2px 0px #6c757d; /* Shadow for depth */
    }

    /* Navbar style */
    nav {
        display: flex;
        gap: 30px;
        margin: 10px 0 40px;
    }

    nav a {
        font-size: 1.5em;
        text-decoration: none;
        color: #f8f9fa; /* Light color for contrast */
        padding: 5px 15px;
        border: 2px solid #ffc107; /* Gold-like border */
        border-radius: 10px;
        background-color: rgba(255, 193, 7, 0.1); /* Transparent goldish background */
        transition: all 0.3s ease;
    }

    nav a:hover {
        background-color: #ffc107; /* Highlight on hover */
        color: #2c2c2c; /* Dark text on hover */
    }

    /* Mascot style */
    .mascot-container {
        width: 300px;
        height: 300px;
        border: 2px solid #6c757d; /* Slight border to frame */
        border-radius: 15px;
        overflow: hidden;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5); /* Depth effect */
    }

    .mascot-container img {
        width: 100%;
        height: 100%;
        object-fit: cover;
    }

    .post {
        background-color: rgba(255, 255, 255, 0.8);
        margin: 10px 0;
        padding: 10px;
        border: 1px solid #ccc;
        border-radius: 4px;
    }

    .post h3 {
        margin: 0;
        font-size: 1.2rem;
    }

    .post p {
        font-size: 1rem;
    }

    #container {
        max-width: 600px;
        margin: 0 auto;
    }
</style>

<main>
    <header>VarmAI</header>
    <nav>
        <a href="#dexscreener">DexScreener</a>
        <a href="#proof-of-consciousness">Proof of Consciousness</a>
        <a href="#white-paper">White Paper</a>
    </nav>
    <div class="mascot-container">
        <img src="/varmcat.png" alt="VarmAI Mascot">
    </div>
    <!--
    <h1>Latest Posts</h1>
    <div id="container">
        {#each posts as post (post.id)}
        <div class="post">
            <h3>{post.title}</h3>
            <p>{post.body}</p>
        </div>
        {/each}
    </div>
    -->
</main>
<!--
<div id="particles-js"></div>
-->

