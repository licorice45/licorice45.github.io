---
title: Home
layout: default
header: home
---
{% include itembox_style.html %}
<div class="grid_container3">
<div class="panelbox mobile-span3">
	<p>Yahoy !!<br>
	I'm <b>licorice45</b>, I can be considered an artist and wannabe programmer<br>
	Also my lucky number is 45<br>
	I'm bad at writing descriptions<br>
	<br>
	Welcome to my website !!</p>
</div>

<div class="itembox mobile-span3" onclick="location.href='/links';" onauxclick="window.open('/links');">
	<div class="ib-item4"><p>Links to Socials & More</p></div>
</div>

<div class="mobile-hide" style="grid-column: 3; grid-row: 1 / span 2; margin: auto;">
	<img src="/assets/sprites/licorice_fall.png">
</div>
</div>

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
	document.getElementById('splash').innerHTML = "\"" + splash[rng] + "\"";
</script>

# Check out my...
<div class="grid_container3">
	<div class="itembox" onclick="location.href='/projects/marzipan';" onauxclick="window.open('/projects/marzipan');">
		<div class="ib-item4"><img class="itembox-thumb" src="/assets/sprites/projects/banner_Marzipan.png"></div>
		<div class="ib-item5"><p>Featured Project:<br><b>Marzipan</b></p></div>
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

<div class="panelbox">
	<h2>Friend-sites !! :D</h2>
	<div class="grid_container3">
		{% for link in site.data.links_friends %}
		<div class="itembox" onclick="location.href='{{ link.url }}';" onauxclick="window.open('{{ link.url }}');" style="--c: {{ link.bgcolor }}; background-image: url({{ link.image }});">
			<div class="ib-item4"><p><b>{{ link.name }}</b></p></div>
		</div>
		{% endfor %}
	</div>
</div>
