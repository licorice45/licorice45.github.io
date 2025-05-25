---
title: Home
layout: default
---
{% include splash_text.html %}

## About

<div class="grid-container-3">
<div class="card mobile-span-3">
	<p>Yahoy !!<br>
	I'm <b>licorice45</b>, I can be considered an artist and wannabe programmer!<br>
	This website's main purpose to provide quick access to my links, projects and more.<br>
	<br>
	Enjoy your stay !!</p>
</div>

{% include button.html url="/links" class="mobile-span-3" content="Links to Socials & More" %}

<div class="mobile-hide" style="grid-column: 3; grid-row: 1 / span 2; margin: auto;">
	<img src="/assets/sprites/licorice_fall.png">
</div>
</div>

## Check out
<div class="grid-container-3">
	{% include squarelink.html url="/projects/marzipan" image="/assets/sprites/projects/thumbnail_Marzipan.png" name="<b>Featured Project</b><br>Marzipan" %}
	{% include squarelink.html url="/projects" image="/assets/sprites/thumbnail_projects.png" name="Other Projects" %}
	{% include squarelink.html url="/ocs" image="/assets/sprites/thumbnail_ocs.png" name="Original Characters" %}
</div>


## Friend-sites
<div class="grid-container-2">
	{% for link in site.data.links_friends %}
		{% capture url %}{{ link.url }}{% endcapture %} {% capture color %}{{ link.bgcolor }}{% endcapture %} {% capture bg-image %}{{ link.image }}{% endcapture %} {% capture content %}{{ link.name }}{% endcapture %}
		{% include friend.html href=url color=color bg-image=bg-image name=content %}
	{% endfor %}
</div>
