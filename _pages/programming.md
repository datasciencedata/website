---
layout: page
title: Programming Posts!!
permalink: /programming/
description: Learn about most popular programming languages for data science such as Python and R. You will find easy way to learn coding and analyze data with this programming skill.
---

<div class="post-list">

{% for category in site.categories %}
    {% capture category_name %}{{ category | first }}{% endcapture %}
        {% if category_name=="programming" %}
             {% for post in site.categories[category_name] %}
                 {% include card.html %}
             {% endfor %}
        {% endif %}
{% endfor %}

</div>
