---
title: Gallery
layout: page
---

{% for image in site.gallery %}
<div class="row">
    <div class="col-md-4">
        <a href="{{ image.filename }}"><h3>{{ image.title }}</h3></a>
        {{ image.content }}
    </div>
    <div class="col-md-8">
        <a href="{{ image.filename }}"><span class="image fit"><img src="images/{{ image.img }}" alt="" /></span></a>
    </div>
</div>
<hr>
{% endfor %}