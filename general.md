---
layout: default
title: General
subtitle: Posts about general topics that don't fall under other categories
---
<h1>Simple Category Pages with vanilla Jekyll</h1>

{% unless page.content == '' %}
  <p>{{ page.content }}</p>
{% endunless %}

{% for post in site.categories.general %}
  <h2><a href=""></a></h2>
  <p></p>
{% endfor %}
