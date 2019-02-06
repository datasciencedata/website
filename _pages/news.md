---
layout: page
title: Machine Learning Model!!
permalink: /news/
description: Stay up to date with the latest trend and news of data science and artificial intelligence. Get the latest tech news and important update of data science domain.
---

<div class="post-list">

{% for category in site.categories %}
    {% capture category_name %}{{ category | first }}{% endcapture %}
        {% if category_name=="news" %}
             {% for post in site.categories[category_name] %}
                 {% include card.html %}
             {% endfor %}
        {% endif %}
{% endfor %}

</div>
              