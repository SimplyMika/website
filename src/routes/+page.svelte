<script>
	import { resolve } from "$app/paths";
</script>

<header>
	<div>
		<h1>Hi, I'm Mika.</h1>
		<h2>I make good software.</h2>
	</div>
	<div>
		<a href={resolve("/hire-me")}>Hire me</a>
	</div>
</header>

<style>
	header {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		align-items: start;
		gap: 2em;

		padding-block: 4em;
	}
	@container (width < 32rem) {
		header {
			flex-direction: column;
		}
	}

	h1,
	h2 {
		margin: 0;
		line-height: 1.5;
	}

	a {
		display: block;

		background-color: var(--coral);
		color: var(--white);
		border: none;
		cursor: pointer;
		font-weight: bold;

		padding: 1em;
		font-size: 1.5em;

		text-wrap-mode: nowrap;
	}

	a:hover {
		background: var(--white);
		color: var(--coral);
	}
</style>
