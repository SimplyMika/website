<script>
	import { resolve } from "$app/paths";
</script>

<header>
	<div>
		<h1>Hi, I'm Mika.</h1>
		<h2>I make <strong>good software</strong>.</h2>
	</div>
	<div>
		<a href={resolve("/hire-me")}>Hire me</a>
	</div>
</header>
<section id="technologies">
	<h2><a href="#technologies">#1</a> Technologies I've worked with</h2>
	<ul>
		<li>Angular</li>
		<li>ASP.NET</li>
		<li>AutoHotkey</li>
		<li>Bun</li>
		<li>C</li>
		<li>C#</li>
		<li>ClickUp</li>
		<li>Dart</li>
		<li>Deno</li>
		<li>Docker</li>
		<li>Docker Compose</li>
		<li>Figma</li>
		<li>Flutter</li>
		<li>Fly.io</li>
		<li>Git</li>
		<li>GitHub Actions</li>
		<li>Gradle</li>
		<li>Java</li>
		<li>JavaScript</li>
		<li>Jira</li>
		<li>Kotlin/JVM</li>
		<li>Kotlin/Multiplatform</li>
		<li>Ktor</li>
		<li>Kubernetes</li>
		<li>Linux</li>
		<li>Maven</li>
		<li>Node</li>
		<li>Python</li>
		<li>React</li>
		<li>React Native</li>
		<li>Spring Boot</li>
		<li>Svelte</li>
		<li>SvelteKit</li>
		<li>Trello</li>
		<li>TypeScript</li>
		<li>Vercel</li>
		<li>Vue</li>
		<li>Windows</li>
		<li>Zig</li>
	</ul>
</section>
<section id="focuses">
	<h2><a href="#focuses">#2</a> Things I focus on in my work</h2>
	<h3>Correctness</h3>
	<p>
		If there's one thing I hate, it's <strong>bugs</strong>. That's why I always try to consider every edge-case that could
		possibly happen and account for them all. And I like to think that I'm pretty good at that!
	</p>
	<h3>Maintainability</h3>
	<p>
		Another thing I can't stand is reading <strong>shitty code</strong>. To spare myself and others from that, my code is always
		as readable as I can make it. I'd rather spend an extra few minutes now, than an extra few <strong>hours</strong> later.
	</p>
	<h3>Performance</h3>
	<p>
		Reload this page. Go ahead, it won't take long. And that's precisely the point! I love things that are
		<strong>fast and snappy</strong>, and all of my software is.
	</p>
</section>
<section id="projects">
	<h2><a href="#projects">#3</a> Personal projects I'm most proud of</h2>
	<h3>TransL</h3>
	<p>
		TransL is a Discord translation bot. It features deep integration into the Discord ecosystem via Slash Commands, and it
		translates messages via the hugely popular and particularly accurate DeepL Translator.
	</p>
	<p>
		It's written in pure Kotlin with the Kord framework, which I extended with my own purpose-built functions and classes. It's
		hosted on a VPS in a Docker container.
	</p>
	<p>Have a look on <a href="https://github.com/SimplyMika/transl">GitHub</a>.</p>
	<h3>Twirl</h3>
	<p>Twirl brings a whole bunch of different loading spinner designs for the commandline into the Zig ecosystem.</p>
	<p>
		Its API is extremely flexible with every possible use-case being possible, be it a dead-simple sleep-loop or highly complex
		custom display logic.
	</p>
	<p>Twirl is hosted on <a href="https://codeberg.org/SimplyMika/twirl">Codeberg</a>.</p>
	<h3>libautomate</h3>
	<p>
		libautomate is a Zig library for desktop automation on Windows, MacOS, and Linux. It's part of a bigger project called
		NeoHotkey, which will be a fully modernized replacement of the scripting language AutoHotkey (once it's finished).
	</p>
	<p>libautomate is far from complete as of yet.</p>
	<p>
		You can find the project on <a href="https://codeberg.org/NeoHotkey/libautomate">Codeberg</a>.
	</p>
</section>

<style>
	header {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		align-items: start;
		gap: 2em;

		margin-block: 4em;
	}
	@container (width < 32rem) {
		header {
			flex-direction: column;
		}
	}

	header h1,
	header h2 {
		margin: 0;
		line-height: 1.5;
	}

	header a {
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

	header a:hover {
		background: var(--white);
		color: var(--coral);
	}

	section {
		margin-block: 2em;
	}

	ul {
		display: flex;
		flex-wrap: wrap;
		gap: 0.5em;

		list-style: none;
		margin: 0;
		padding: 0;
	}

	ul li {
		padding: calc(1em - 1px);
		border: 1px solid var(--coral);
		box-sizing: border-box;
		line-height: 1em;
		text-align: center;

		width: fit-content;
		width: calc-size(fit-content, round(up, size, 2em));
	}
</style>
