---
layout: page
title: Categories
permalink: /categories/
---

<div>
{% assign categories = site.categories | sort %}
  {% for category in categories %}
    <div class="archive-group">
      {% capture category_name %}{{ category | first }}{% endcapture %}
      <div id="#{{ category_name | slugize }}"></div>
      <p></p>
      <a name="{{ category_name | slugize }}"></a>
      <div class="container">
        <h1 class="category-head">{{ category_name }}</h1>
        <div class="post-list-categories" itemscope="" itemtype="http://schema.org/Blog">
          {% for post in site.categories[category_name] %}
            {% include card-categories.html %}
          {% endfor %}
          <!-- {% include pagination.html %} -->
        </div>
      </div>
    </div>
  {% endfor %}
</div>