---
layout: page
title: Events
---

### Current Events
{% for event in site.events %}
{% if event.state == "current" %}
>
#### {{ event.title }}
{{ event.abstract }}<br>
[Read More]({{ site.url }}/events/{{ event.eventid }})
{% endif %}
{% endfor %}

### Completed Events
{% for event in site.events %}
{% if event.state == "past" %}
>
#### {{ event.title }}
{{ event.abstract }}<br>
[Read More]({{ site.url }}/events/{{ event.eventid }})
{% endif %}
{% endfor %}


### Future Events
{% for event in site.events %}
{% if event.state == "future" %}
>
#### {{ event.title }}
{{ event.abstract }}<br>
[Read More]({{ site.url }}/events/{{ event.eventid }})
{% endif %}
{% endfor %}