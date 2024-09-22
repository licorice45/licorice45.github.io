---
title: Home
layout: default
header: home
---
{% include itembox_style.html %}
<div class="grid_container3">
<div class="panelbox" style="grid-column: 1 / span 2;">
	<p>Yahoy !!<br>
	I'm <b>licorice45</b>, I can be considered an artist and wannabe programmer<br>
	Also my lucky number is 45<br>
	I'm bad at writing descriptions<br>
	<br>
	Welcome to my website !!</p>
</div>

<div class="itembox" onclick="location.href='/links';" onauxclick="window.open('/links');" style="grid-column: 1 / span 2;">
	<div class="ib-item4"><p>Links to Socials & More</p></div>
</div>

<div style="grid-column: 3; grid-row: 1 / span 2; margin: auto;">
	<img src="/assets/sprites/licorice_fall.png">
</div>
</div>

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
