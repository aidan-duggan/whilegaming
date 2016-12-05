---
layout: page
title: archive
subtitle: Posts by tag
---

# Archive
Click on each post title to view it.
_Under Construction_

{% for type in site.type %}
  <h2 class='tag-header' id="{{ type[0] }}-ref">{{ type[0] }}</h2>
  <ul>
    {% assign pages_list = type[1] %}

    {% for node in pages_list %}
      {% if node.title != null %}
        {% if group == null or group == node.group %}
          {% if page.url == node.url %}
          <li class="active"><a href="{{node.url}}" class="active">{{node.title}}</a></li>
          {% else %}
          <li><a href="{{node.url}}">{{node.title}}</a></li>
          {% endif %}
        {% endif %}
      {% endif %}
    {% endfor %}

    {% assign pages_list = nil %}
    {% assign group = nil %}
  </ul>
{% endfor %}
