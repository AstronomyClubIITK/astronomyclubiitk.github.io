---
layout: page
title: Galleria
images:
    -   image_path: images/pic01.jpg
        id: 1
    -   image_path: images/pic02.jpg
        id: 2
    -   image_path: images/pic03.jpg
        id: 3
---


<div class="row">
<ul class="slides">
{% for image in page.images %}
    <input type="radio" name="radio-btn" id="{{ image.id }}" checked />
    <li class="slide-container">
		<div class="slide">
			<img src="{{image.image_path}}" />
        </div>
		<div class="nav">
            {% if image.prev %}<label for="{{ image.prev.id }}" class="prev">&#x2039;</label>{% endif %}
			{% if image.next %}<label for="{{image.next.id}}" class="next">&#x2039;</label>{% endif %}
		</div>
        <div id="fb_comments" >
            <div class="fb-comments" data-href="{{ site.url }}/gallery/{{ image.image_path }}" data-colorscheme="dark" data-num-posts="4" data-width="100%"></div>
        </div>
    </li>
{% endfor %}
</ul>
</div>