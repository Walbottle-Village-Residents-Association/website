---
layout: default
title: Blog
permalink: /blog/
---
# I am a blog
{% for post in site.posts limit: 3 %}
  <div class="post_info">
    <li>
         <a href="{{ post.url }}">{{ post.title }}</a>
         <span>({{ post.date | date:"%Y-%m-%d" }})</span>
    </li>
    </div>
  {% endfor %}