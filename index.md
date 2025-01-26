---
title: Home
layout: default
---
{% include itembox_style.html %}

<p id="splash">"missingno"</p>
<script>
	const splash = [
		"Removed Herobrine",
		"I love Pesto mmm yummy",
		"45",
		"Yo, Angelo",
		"You should watch Mob Psycho 100 rn",
		"This site was made using notepad",
		"Press THROW and then JUMP to throw Salmon Eggs further",
		"Eh? Is that a... TURRÓN?!",
		"Why are oranges called orange but apricots aren't called orange 🤯",
		"I can't stop procrastinating, HELP",
		"Searing Shells by Kojimkj, best stage",
		"Let the shackles be released!",
		"I... am licorice",
		"Awesome orb of awesomeness",
		"Give me a drink, bartender"
	];
	
	const rng = Math.floor(Math.random() * splash.length);
	document.getElementById('splash').innerHTML = "<b>\"" + splash[rng] + "\"";
</script>

## About

<div class="grid_container3">
<div class="panelbox mobile-span3">
	<p>Yahoy !!<br>
	I'm <b>licorice45</b>, I can be considered an artist and wannabe programmer!<br>
	This website's main purpose to provide quick access to my links, projects and more.<br>
	<br>
	Enjoy your stay !!</p>
</div>

<div class="itembox mobile-span3" onclick="location.href='/links';" onauxclick="window.open('/links');">
	<div class="ib-item4"><p>Links to Socials & More</p></div>
</div>

<div class="mobile-hide" style="grid-column: 3; grid-row: 1 / span 2; margin: auto;">
	<img src="/assets/sprites/licorice_fall.png">
</div>
</div>

## Check out
<div class="grid_container3">
	<div class="itembox" onclick="location.href='/projects/marzipan';" onauxclick="window.open('/projects/marzipan');">
		<div class="ib-item4"><img class="itembox-thumb" src="/assets/sprites/projects/banner_Marzipan.png"></div>
		<div class="ib-item5"><p><b>Featured Project</b><br>Marzipan</p></div>
	</div>
	<div class="itembox" onclick="location.href='/projects';" onauxclick="window.open('/projects');">
		<div class="ib-item4"><img class="itembox-thumb" src="/assets/sprites/banner_projects.png"></div>
		<div class="ib-item5"><p>Other Projects</p></div>
	</div>
	<div class="itembox" onclick="location.href='/ocs';" onauxclick="window.open('/ocs');">
		<div class="ib-item4"><img class="itembox-thumb" src="/assets/sprites/banner_ocs.png"></div>
		<div class="ib-item5"><p>Original Characters</p></div>
	</div>
</div>


## Friend-sites
<div class="grid_container2">
	{% for link in site.data.links_friends %}
	<div class="itembox" onclick="location.href='{{ link.url }}';" onauxclick="window.open('{{ link.url }}');" style="--c: {{ link.bgcolor }}; background-image: url({{ link.image }});">
		<div class="ib-item4"><p>{{ link.name }}</p></div>
	</div>
	{% endfor %}
</div>
