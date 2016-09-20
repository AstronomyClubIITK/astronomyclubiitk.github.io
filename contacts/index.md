---
layout: page
title: Contact Us
---
<div class="container">
<div class="row">
    <div class="col-md-6">
        <iframe src="https://docs.google.com/forms/d/1fmVIMAIWBlQewWmGbRNCMFPlr3rzZrzU1GU7D9ZpXKI/viewform?embedded=true" height="480px" width="100%">Loading...</iframe>
    </div>
    <div class="col-md-6">
        <iframe  width="100%" height="320px" scrolling="no" marginheight="0" src="https://maps.google.com/maps?f=q&amp;source=s_q&amp;hl=en&amp;geocode=&amp;ll=26.504806,80.229129&amp;spn=0.01628,0.025663&amp;z=18&amp;iwloc=A&amp;output=embed"></iframe>
        Room 401 <br>
        Roof Top <br>
        New Sac <br>
        IIT Kanpur
    </div>
</div>
<hr>
<h2>Coordinators</h2>
<div class="row">
{% for contact in site.contacts %}
    {% if contact.coordinator  %}
        <div id="{{ contact.authorid }}" class="col-md-3 col-sm-3 col-lg-3">
            {% if contact.img %}
                <img class="img img-circle" src="{{ site.url }}/contacts/images/{{ contact.img }}" width="100%" />
            {% else %}
                <img class="img img-circle" src="{{ site.url }}/contacts/images/placeholder.jpg" width="100%"/>
            {% endif %}
            <center>{{ contact.name }}
            {% if contact.phone %}<br>Phone: {{contact.phone}}{%endif%}
            {% if contact.mail %}<br><a href="mailto:{{contact.mail}}" target="_blank">{{contact.mail}}</a>{%endif%}
            {% if contact.facebook %}<br><a target="_blank" href="{{contact.facebook}}" class="icon fa-facebook"></a>{% endif %}
            {% if contact.twitter %}<a target="_blank" href="{{contact.twitter}}" class="icon fa-twitter"></a>{% endif %}
            {% if contact.github %}<a target="_blank" href="{{contact.github}}" class="icon fa-github"></a>{% endif %}
            </center>
        </div>
    {% endif %}
{% endfor %}
</div>
<hr>
<h2>Secretaries</h2>
<div class="row">
{% for contact in site.contacts %}
    {% if contact.secretary  %}
        <div id="{{ contact.authorid }}" class="col-md-3 col-sm-3 col-lg-3">
            {% if contact.img %}
                <img class="img img-circle" src="{{ site.url }}/contacts/images/{{ contact.img }}" width="100%" />
            {% else %}
                <img class="img img-circle" src="{{ site.url }}/contacts/images/placeholder.jpg" width="100%"/>
            {% endif %}
            <center>{{ contact.name }}
            {% if contact.phone %}<br>Phone: {{contact.phone}}{%endif%}
            {% if contact.mail %}<br><a href="mailto:{{contact.mail}}" target="_blank">{{contact.mail}}</a>{%endif%}
            {% if contact.facebook %}<br><a target="_blank" href="{{contact.facebook}}" class="icon fa-facebook"></a>{% endif %}
            {% if contact.twitter %}<a target="_blank" href="{{contact.twitter}}" class="icon fa-twitter"></a>{% endif %}
            {% if contact.github %}<a target="_blank" href="{{contact.github}}" class="icon fa-github"></a>{% endif %}
            </center>
        </div>
    {% endif %}
{% endfor %}
</div>
<hr>
<h2>Other Members</h2>
<div class="row">
{% for contact in site.contacts %}
    {% if contact.coordinator  %}
    {% elsif contact.secretary %}
    {% else %}
        <div id="{{ contact.authorid }}" class="col-md-3 col-sm-3 col-lg-3">
            {% if contact.img %}
                <img class="img img-circle" src="{{ site.url }}/contacts/images/{{ contact.img }}" width="100%" />
            {% else %}
                <img class="img img-circle" src="{{ site.url }}/contacts/images/placeholder.jpg" width="100%"/>
            {% endif %}
            <center>{{ contact.name }}
            {% if contact.phone %}<br>Phone: {{contact.phone}}{%endif%}
            {% if contact.mail %}<br><a href="mailto:{{contact.mail}}" target="_blank">{{contact.mail}}</a>{%endif%}
            {% if contact.facebook %}<br><a target="_blank" href="{{contact.facebook}}" class="icon fa-facebook"></a>{% endif %}
            {% if contact.twitter %}<a target="_blank" href="{{contact.twitter}}" class="icon fa-twitter"></a>{% endif %}
            {% if contact.github %}<a target="_blank" href="{{contact.github}}" class="icon fa-github"></a>{% endif %}
            </center>
        </div>
    {% endif %}
{% endfor %}
</div>
</div>