---
layout: page
title: playing
subtitle: A record of games I have played
css: "/css/index.css"
---
<div>
  {% for game in site.games %}        
    <div class="clearfix float-my-children">
       <img src="//upload.wikimedia.org/wikipedia/commons/thumb/6/6e/Balzac.jpg/220px-Balzac.jpg" width=100></img> <div>{{ game.game }}</div>
    </div>
  {% endfor %}
</div>
