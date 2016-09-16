---
layout: page
title: Can You answer these?
---
{% for challenge in site.challenges %}
<h3>{{ challenge.challengeid }}. {{ challenge.title }}</h3>
{{ challenge.content }}
<a href="{{ site.url }}/challenges/{{ challenge.challengeid }}"><button class="btn btn-default">Answer >></button></a>
<hr>
{% endfor %}