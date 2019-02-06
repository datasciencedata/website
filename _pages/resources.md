---
layout: page
title: Get Everything You Need !!
permalink: /learning-resource/
description: Get whatever you need in order to kickstart your data science journey. Know about top free videos, articles, books and courses abailable around the web.
---

<div class="post-list">

{% for category in site.categories %}
    {% capture category_name %}{{ category | first }}{% endcapture %}
        {% if category_name=="learning-resources" %}
             {% for post in site.categories[category_name] %}
                 {% include card.html %}
             {% endfor %}
        {% endif %}
{% endfor %}

</div>