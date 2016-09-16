---
layout: page
title: Projects
---

### Current Projects
{% for project in site.projects %}
{% if project.state == "current" %}
>
#### {{ project.title }}
{{ project.abstract }}<br>
[Read More]({{ site.url }}/projects/{{ project.projectid }})
{% endif %}
{% endfor %}

### Completed Projects
{% for project in site.projects %}
{% if project.state == "completed" %}
>
#### {{ project.title }}
{{ project.abstract }}<br>
[Read More]({{ site.url }}/projects/{{ project.projectid }})
{% endif %}
{% endfor %}


### Prospective Projects
{% for project in site.projects %}
{% if project.state == "prospective" %}
>
#### {{ project.title }}
{{ project.abstract }}<br>
[Read More]({{ site.url }}/projects/{{ project.projectid }})
{% endif %}
{% endfor %}