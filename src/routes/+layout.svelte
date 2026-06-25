<script lang="ts">
	import { resolve } from "$app/paths";
	import { page } from "$app/state";
	import favicon from "$lib/assets/favicon.svg";

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<div class="page">
	<header>
		<a class="mika" href={resolve("/")}>Mika</a>
		<nav>
			<a href={resolve("/me")} class:active={page.url.pathname == resolve("/me")}>me</a>
			<a href={resolve("/projects")} class:active={page.url.pathname == resolve("/projects")}>projects</a>
		</nav>
	</header>

	<main>
		{@render children()}
	</main>
</div>

<style>
	.page {
		display: grid;
		grid-template-rows: [head] auto [main] 1fr;
		grid-template-columns: min(100%, 64rem);

		justify-content: center;
		gap: 1em;
		padding: 1em;

		background-color: var(--night);

		box-sizing: border-box;
		min-height: 100vh;
	}

	header {
		grid-row: head;

		display: flex;
		flex-direction: row;
		justify-content: space-between;
		align-items: center;
	}

	main {
		grid-row: main;

		container-type: inline-size;
	}

	.mika {
		font-size: 2em;
		font-weight: bold;
	}

	nav {
		display: flex;
		flex-direction: row;
		gap: 1em;
	}

	a.active {
		--highlight-color: var(--shell);
	}
</style>
