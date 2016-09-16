---
layout: page
title: Presentations
---

{% for presentation in site.presentations %}
<h3><a href="{{ site.url }}/presentations/{{ presentation.presentationid }}">
    {{ presentation.title }}
</a></h3>
{{ presentation.content }}
<hr>
{% endfor %}