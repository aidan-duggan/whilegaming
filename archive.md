---
layout: page
title: archive
subtitle: Posts by tag
css: "/css/index.css"
---

# Archive
Click on each post title to view it.
_Under Construction_

<div class="posts-list">
  {% for post in site.posts %}
      <article class="post-preview">
      <a href="{{ post.url | prepend: site.baseurl }}">
  	  <h3 class="post-title">{{ post.title }}</h2>
      </a>  
  
      <p class="post-meta">
        Posted on {{ post.date | date: "%B %-d, %Y" }}
      </p>      
        </article>
  {% endfor %}
</div>
