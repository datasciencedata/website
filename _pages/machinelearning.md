---
layout: page
title: Machine Learning Model!!
permalink: /machine-learning/
description: Build Machine Learning Model. You will learn how to build ML model and do ML project. You will analyze data and build comprehensive machine learning model.
---

<div class="post-list">

{% for category in site.categories %}
    {% capture category_name %}{{ category | first }}{% endcapture %}
        {% if category_name=="machinelearning" %}
             {% for post in site.categories[category_name] %}
                 {% include card.html %}
             {% endfor %}
        {% endif %}
{% endfor %}

</div>
              