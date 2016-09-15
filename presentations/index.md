---
layout: page
title: Presentations
presentations:
    -   iframe: <iframe src='https://onedrive.live.com/embed?cid=4173BB1E418F1249&resid=4173BB1E418F1249%2139850&authkey=AC57JihPqzXXwdU&em=2&wdAr=1.7777777777777777' width='100%' height="400px" frameborder='0'>This is an embedded <a target='_blank' href='https://office.com'>Microsoft Office</a> presentation, powered by <a target='_blank' href='https://office.com/webapps'>Office Online</a>.</iframe>
        title: VHE
        id: 1
    -   iframe: <iframe src='https://onedrive.live.com/embed?cid=4173BB1E418F1249&resid=4173BB1E418F1249%2139850&authkey=AC57JihPqzXXwdU&em=2&wdAr=1.7777777777777777' width='100%' height="400px" frameborder='0'>This is an embedded <a target='_blank' href='https://office.com'>Microsoft Office</a> presentation, powered by <a target='_blank' href='https://office.com/webapps'>Office Online</a>.</iframe>
        title: VHE
        id: 2
---

{% for presentation in page.presentations %}
<h3>{{ presentation.title }}</h3>
{{ presentation.iframe }}
<div id="fb_comments" style="padding-left:5%;padding-right:5%;">
    <div class="fb-comments" data-href="{{ site.url }}/presentations/{{ presentation.id }}" data-colorscheme="light" data-num-posts="4" data-width="100%"></div>
</div>
<hr>
{% endfor %}