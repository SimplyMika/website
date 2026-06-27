<h1>My personal projects</h1>
<hgroup>
	<h2>TransL</h2>
	<p>
		TransL is a Discord <strong>translation bot</strong>. It features deep integration into the Discord ecosystem via Slash
		Commands, and it translates messages via the hugely popular and particularly accurate <strong>DeepL Translator</strong>.
	</p>
	<p>
		It's written in pure Kotlin with the Kord framework, which I extended with my own purpose-built functions and classes. It's
		hosted on a VPS in a Docker container.
	</p>
	<p>Have a look on <a href="https://github.com/SimplyMika/transl">GitHub</a>.</p>
</hgroup>
<hgroup>
	<h2>Twirl</h2>
	<p>
		Twirl brings a whole bunch of different <strong>loading spinner</strong> designs for the commandline into the Zig ecosystem.
	</p>
	<p>
		Its API is extremely flexible with every possible use-case being possible, be it a dead-simple sleep-loop or highly complex
		custom display logic.
	</p>
	<p>Twirl is hosted on <a href="https://codeberg.org/SimplyMika/twirl">Codeberg</a>.</p>
</hgroup>
<hgroup>
	<h2>libautomate</h2>
	<p>
		libautomate is a Zig library for <strong>desktop automation</strong> on Windows, MacOS, and Linux. It's part of a bigger
		project called <strong>NeoHotkey</strong>, which will be a fully modernized replacement of the scripting language AutoHotkey
		(once it's finished).
	</p>
	<p>libautomate is far from complete as of yet.</p>
	<p>
		You can find the project on <a href="https://codeberg.org/NeoHotkey/libautomate">Codeberg</a>.
	</p>
</hgroup>
<hgroup>
	<h2>mad</h2>
	<p>
		mad stands for “manipulate any data”. It's a jq-like commandline tool to read, modify, and write data in many different
		formats such as JSON, YAML, TOML, HCON, XML, and several more.
	</p>
	<p>
		It's currently in its early stages and only supports reading files as plain text. It also can't do anything with that data
		yet. It's a proof of concept as of now, but I love the idea so much that I'll probably keep working on it until it's
		finished!
	</p>
	<p>
		Find mad's Zig source code on <a href="https://codeberg.org/SimplyMika/mad">Codeberg</a>.
	</p>
</hgroup>

<style>
	hgroup {
		border: 1px solid var(--coral);
		margin-block: 1em;
		padding: 1em;
	}

	hgroup > :first-child {
		margin-block-start: 0;
	}
	hgroup > :last-child {
		margin-block-end: 0;
	}

	h2 {
	}
</style>
