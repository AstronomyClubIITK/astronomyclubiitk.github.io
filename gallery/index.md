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
<div class="col-md-12">
<ul class="slides ">
{% for image in page.images %}
    <input type="radio" name="radio-btn" id="{{ image.id }}" checked />
    
    <li class="slide-container">
                
                <div class="slide row">
                    <img src="{{image.image_path}}" class="col-md-12"/>
                </div>
                <div class="nav">
                    {% if image.id != 1 %}<label for="{{ image.id | plus: -1}}" class="prev">&#x2039;</label>{% endif %}
                    {% if image.id != 3 %}<label for="{{image.id | plus: 1}}" class="next">&#x203a;</label>{% endif %}
                </div>
                
    </li>
{% endfor %}
</ul>
</div>
</div>