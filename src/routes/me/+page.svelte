<script>
	import { resolve } from "$app/paths";
	import { differenceInYears } from "date-fns";
</script>

<h1>Hi, nice to meet you!</h1>
<p>My real name is <strong>Micha</strong>, but I like to be called Mika in English.</p>
<p>Either way, <strong>I'm pleased to meet you!</strong></p>

<h2>Some stuff about me</h2>
<p>
	I'm a {differenceInYears(new Date(), "2001-12-01")}-year old guy from Germany living in a tiny village somewhere in
	Rhineland-Palatinate.
</p>
<p>
	I'm a software developer out of passion. That means I <strong>love</strong> writing software, and I do it nearly every day.
</p>
<p>
	Software development is my hobby, and it used to be my job, except that I'm currently unemployed. I'd really like to change
	that, so please <a href={resolve("/hire-me")}>hire me</a>!
</p>
<p>
	When I'm not coding, I like to meet up with my friends or play video games. You can occasionally also find me in the gym
	working out or playing Table Tennis.
</p>
