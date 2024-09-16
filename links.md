---
title: Links
layout: default
header: links
---

{% include itembox_style.html %}
# Main
<div class="grid_container3">
{% for link in site.data.links_main %}
{% include itembox_links.html %}
{% endfor %}
</div>
# Misc
<div class="grid_container3">
{% for link in site.data.links_misc %}
{% include itembox_links.html %}
{% endfor %}
</div>
