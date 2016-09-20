---
layout: page
title: Hidden Posts
description: You really shouldn't be here!
---

{% for post in site.posts %}
{% if post.state == "hidden" %}
#### {{ post.title }}
{{post.date | date: '%B %d, %Y'}}
{% if post.author %}<br><a href="{{ site.url }}/contacts/#{{ post.authorid }}" target="_blank">{{ post.author }}</a>{%endif%}
{% if post.img %}
<div class="row">
<div class="col-md-6 col-sm-6">
<span class="image fit"><img src="{{ site.url }}/postimages/{{ post.img }}" alt="" /></span>
</div>
<div class="col-md-6 col-sm-6">
{{ post.abstract }}<br><br>
<a href="{{ site.url }}{{ post.url }}"><button class="btn btn-default">Read More >></button></a>
</div>
{% else %}
{{ post.abstract }}<br><br>
<a href="{{ site.url }}{{ post.url }}"><button class="btn btn-default">Read More >></button></a>
{% endif %}
<hr>
{% endif %}
{% endfor %}