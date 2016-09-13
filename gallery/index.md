---
layout: page
title: Galleria
images:
    - image_path: images/pic01.jpg
    - image_path: images/pic02.jpg
    - image_path: images/pic03.jpg
---

{% for image in page.images %}
<div class="row">
    <div class="image col-md-8">
        <img src="{{image.image_path}}" width="100%"/>
    </div>
    <div class="col-md-4">
        <div id="fb_comments">
            <div class="fb-comments" data-href="{{ site.url }}/gallery/{{ image.image_path }}" data-colorscheme="dark" data-num-posts="4" data-width="100%"></div>
        </div>
    </div>
</div>
{% endfor %}

