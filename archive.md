---
layout: page
title: archive
subtitle: Posts by tag
css: "/css/index.css"
---

<div class="posts-list">
  {% for post in site.posts %}
      <a href="{{ post.url | prepend: site.baseurl }}">
  	  <p class="post-title">      
        {{ post.date | date: "%B %-d, %Y" }} - {{ post.title }}</p>
      </a>  
  {% endfor %}
</div>
