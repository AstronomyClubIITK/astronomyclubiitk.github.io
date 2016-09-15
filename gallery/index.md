---
title: Gallery
layout: page
---

{% for image in site.gallery %}
<div class="row">
    <div class="col-md-8">
        <span class="image fit"><img src="{{ image.img }}" alt="" /></span>
    </div>
    <div class="col-md-4">
        <h3>{{ image.title }}</h3>
        {{ lu.content }}
    </div>
</div>
<div id="fb_comments" style="padding-left:5%;padding-right:5%;padding-bottom:10%">
    <div class="fb-comments" data-href="{{ site.url }}/gallery/{{ gallery.title }}" data-colorscheme="light" data-num-posts="4" data-width="100%"></div>
</div>
{% endfor %}