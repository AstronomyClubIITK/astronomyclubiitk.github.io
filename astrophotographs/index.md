---
title: Astro Photographs
layout: page
---

{% for image in site.astrophotographs %}
<div class="row">
    <div class="col-md-4">
        <a href="{{ site.url }}/astrophotographs/{{ image.imageid }}"><h3>{{ image.imageid }}. {{ image.title }}</h3></a>
        {{ image.content }}
    </div>
    <div class="col-md-8">
        <a href="{{ site.url }}/astrophotographs/{{ image.imageid }}"><span class="image fit"><img src="images/{{ image.img }}" alt="" /></span></a>
    </div>
</div>
<a href="{{ site.url }}/astrophotographs/{{ image.imageid }}"><button class="btn btn-default">comments >></button></a>
<hr>
{% endfor %}