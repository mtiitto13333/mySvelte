<script>
	//STARTUP PROCESS
	//1.Start Project "npm degit sveltejs/template project-folder-name"
	//2.Direct to folder name
	//3. "npm install"
	//4. run the "npm run dev" in the command prompt to get 
	//local host link for website viewing
	export let name;
	import Greeting from './Greeting.svelte';
	import Math from './Math.svelte';
	let user = {loggedIn: false}
	function loggedinToggle(){
		user.loggedIn = !user.loggedIn;
	}
</script>

<main>
{#if user.loggedIn}
	<button on:click={loggedinToggle}>Log Out</button>
	
	<h1>Hello {name}!</h1>
	<h2>wvgoieuvwgwilv</h2>
{:else }
	<button on:click={loggedinToggle}>Log In</button>
{/if}	
	<Greeting firstName= '' lastName=''/>
	<Math />
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
</style>