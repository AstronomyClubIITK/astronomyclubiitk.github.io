---
layout: page
title: Presentations
---

{% for presentation in site.presentations %}
<h3><a href="{{ site.url }}/presentations/{{ presentation.presentationid }}">
    {{ presentation.presentationid }}. {{ presentation.title }}
</a></h3>
{{ presentation.content }}
<a href="{{ site.url }}/presentations/{{ presentation.presentationid }}"><button class="btn btn-default">comments >></button></a>
<hr>
{% endfor %}