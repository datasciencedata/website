---
layout: page
title: Data Science Posts!!
permalink: /data-science/
description: Learn about data science and various techniques to perform data analysis, wrangling, pre-processing and so on. Get insightful view of data science with some exclusive articles.
---

<div class="post-list">

{% for category in site.categories %}
    {% capture category_name %}{{ category | first }}{% endcapture %}
        {% if category_name=="datascience" %}
             {% for post in site.categories[category_name] %}
                 {% include card.html %}
             {% endfor %}
        {% endif %}
{% endfor %}

</div>


              