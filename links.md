---
title: Links
desc: Quick access collection of links
layout: default
---
## Main
<div class="grid-container-3">
{% for link in site.data.links_main %}
{% include itembox_links.html %}
{% endfor %}
</div>
## Misc
<div class="grid-container-3">
{% for link in site.data.links_misc %}
{% include itembox_links.html %}
{% endfor %}
</div>
