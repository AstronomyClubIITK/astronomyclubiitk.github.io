---
layout: page
title: Galleria
images:
    -   image_path: images/pic01.jpg
        id: 1
        description: description/pic01.html
    -   image_path: images/pic02.jpg
        id: 2
        description: description/pic01.html
    -   image_path: images/pic03.jpg
        id: 3
        description: description/pic01.html
---
Here are a few of the many images we click at astronomy club. 


(For best experience please use a desktop browser)
<div style="height:1080px; display:block;overflow:scroll">
<ul class="slides ">
{% for image in page.images %}
    <input type="radio" name="radio-btn" id="{{ image.id }}" checked />
    <li class="slide-container">
        <div class="slide">
            <img src="{{image.image_path}}"/>
            <div class="row">
                <div class="col-md-8">
                    <iframe width="100%" height="360px" display="block" overflow="scroll" src="{{ image.description }}" ></iframe>
                </div>
                <div class="col-md-4">
                    <div id="fb_comments">
                        <div class="fb-comments" data-href="{{ site.url }}/gallery/{{ image.image_path }}" data-colorscheme="dark" data-num-posts="4" data-width="100%"></div>
                    </div>
                </div>
            </div>
        </div>
        <div class="nav">
            {% if image.id != 1 %}<label for="{{ image.id | plus: -1}}" class="prev">&#x2039;</label>{% endif %}
            {% if image.id != 3 %}<label for="{{image.id | plus: 1}}" class="next">&#x203a;</label>{% endif %}
        </div>
    </li>
{% endfor %}
</ul>
</div>
