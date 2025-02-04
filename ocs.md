---
title: Characters
desc: Archive of licorice45's original characters
layout: default
---
{% assign ocs = site.ocs | sort:"order" %}
{% for oc in ocs %}
{% capture url %}{{ oc.url }}{% endcapture %} {% capture image %}/assets/sprites/ocs/thumbnail_{{ oc.title | downcase }}.png{% endcapture %} {% capture title %}{{ oc.title }}{% endcapture %} {% capture desc %}{{ oc.desc }}{% endcapture %}
{% include itembox.html url=url item1=image item2=title item3=desc %}
{% endfor %}
