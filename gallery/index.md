---
title: Gallery
layout: page
---

{% for image in site.gallery %}
<div class="row">
    <div class="col-md-4">
        <a href="{{ image.title }}.html"><h3>{{ image.title }}</h3></a>
        {{ image.content }}
    </div>
    <div class="col-md-8">
        <a href="{{ image.title }}.html"><span class="image fit"><img src="{{ image.img }}" alt="" /></span></a>
    </div>
</div>
<div id="fb_comments" style="padding-left:5%;padding-right:5%;padding-bottom:10%">
    <div class="fb-comments" data-href="{{ site.url }}/gallery/{{ image.title }}" data-colorscheme="light" data-num-posts="4" data-width="100%"></div>
</div>
<hr>
{% endfor %}