---
title: Links
desc: Quick access collection of links
layout: default
---
## Main
<div class="grid-container-3">
{% for link in site.data.links_main %}
  {% assign name = link.name %}
  {% assign hover = link.hover %}
  {% assign url = link.url %}
  {% assign image = link.image %}
  {% assign bgcolor = link.bgcolor %}
  {% include squarelink.html name=name hover=hover url=url image=image bgcolor=bgcolor %}
{% endfor %}
</div>
## Misc
<div class="grid-container-3">
{% for link in site.data.links_misc %}
  {% assign name = link.name %}
  {% assign hover = link.hover %}
  {% assign url = link.url %}
  {% assign image = link.image %}
  {% assign bgcolor = link.bgcolor %}
  {% include squarelink.html name=name hover=hover url=url image=image bgcolor=bgcolor %}
{% endfor %}
</div>